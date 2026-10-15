---
description: 將所有變更加入暫存區、建立 Commit 並推送至遠端（請謹慎使用）
allowed-tools: Bash(git add:*), Bash(git status:*), Bash(git commit:*), Bash(git push:*), Bash(git diff:*), Bash(git log:*), Bash(git pull:*)
---

# Commit 並推送所有變更

⚠️ **注意**：這會將「所有」變更加入暫存區、建立 Commit，並推送至遠端。只有在確認所有變更應一併提交時才使用。

## 工作流程

### 1. 分析變更
平行執行：
- `git status`——顯示已修改／新增／刪除／未追蹤的檔案
- `git diff --stat`——顯示變更統計
- `git log -1 --oneline`——查看最新 Commit 的訊息格式

### 2. 安全性檢查

**❌ 若偵測到下列內容，請停止並警告：**
- 機密資料：`.env*`、`*.key`、`*.pem`、`credentials.json`、`secrets.yaml`、`id_rsa`、`*.p12`、`*.pfx`、`*.cer`
- API 金鑰：任何含有真實值的 `*_API_KEY`、`*_SECRET`、`*_TOKEN` 變數（不含 `your-api-key`、`xxx`、`placeholder` 等佔位符）
- 大型檔案：未使用 Git LFS 且大小 `>10MB` 的檔案
- 建置產物：`node_modules/`、`dist/`、`build/`、`__pycache__/`、`*.pyc`、`.venv/`
- 暫存檔案：`.DS_Store`、`thumbs.db`、`*.swp`、`*.tmp`

**API 金鑰驗證：**
檢查已修改檔案，尋找以下形式：
```bash
OPENAI_API_KEY=sk-proj-xxxxx  # ❌ 偵測到真實金鑰！
AWS_SECRET_KEY=AKIA...         # ❌ 偵測到真實金鑰！
STRIPE_API_KEY=sk_live_...    # ❌ 偵測到真實金鑰！

# ✅ 可接受的佔位符：
API_KEY=your-api-key-here
SECRET_KEY=placeholder
TOKEN=xxx
API_KEY=<your-key>
SECRET=${YOUR_SECRET}
```

**✅ 請確認：**
- `.gitignore` 設定正確
- 沒有 Merge 衝突
- 目前分支正確（若為 main／master 則警告）
- API 金鑰僅使用佔位符

### 3. 要求確認

顯示摘要：
```
📊 變更摘要：
- 修改 X 個檔案、新增 Y 個、刪除 Z 個
- 總計：新增 +AAA 行、刪除 -BBB 行

🔒 安全性：✅ 無機密資料 | ✅ 無大型檔案 | ⚠️ [警告]
🌿 分支：[name] → origin/[name]

接下來將執行：git add . → commit → push

輸入 'yes' 繼續，或輸入 'no' 取消。
```

**必須等待使用者明確輸入「yes」，才能繼續。**

### 4. 執行（確認之後）

依序執行：
```bash
git add .
git status  # 確認暫存狀態
```

### 5. 產生 Commit 訊息

分析變更，並依 Conventional Commits 規範建立訊息：

**格式：**
```
[type]: 簡短摘要（最多 72 個字元）

- 主要變更 1
- 主要變更 2
- 主要變更 3
```

**類型：** `feat`、`fix`、`docs`、`style`、`refactor`、`test`、`chore`、`perf`、`build`、`ci`

**範例：**
```
docs: 更新概念說明 README，補充完整文件

- 新增架構圖與表格
- 加入實際操作範例
- 擴充最佳實務章節
```

### 6. Commit 與 Push

```bash
git commit -m "$(cat <<'EOF'
[產生的 Commit 訊息]
EOF
)"
git push  # 失敗時：git pull --rebase && git push
git log -1 --oneline --decorate  # 驗證
```

### 7. 確認成功

```
✅ 已成功推送至遠端！

Commit：[hash] [message]
分支：[branch] → origin/[branch]
變更檔案：X（+新增行數、-刪除行數）
```

## 錯誤處理

- **git add 失敗**：檢查權限、鎖定檔案，確認儲存庫已初始化
- **git commit 失敗**：修正 Pre-commit Hooks、檢查 Git 設定（user.name／email）
- **git push 失敗**：
  - 無法 Fast-forward：`git pull --rebase && git push`
  - 沒有遠端分支：`git push -u origin [branch]`
  - 受保護的分支：改用 PR 工作流程

## 何時使用

✅ **適合的情境：**
- 更新多個文件
- 包含測試與文件的功能
- 跨檔案修正錯誤
- 整個專案的格式調整／重構
- 設定變更

❌ **應避免的情境：**
- 不確定將要提交什麼
- 含有機密或敏感資料
- 未經審查就修改受保護分支
- 存在 Merge 衝突
- 希望保留細粒度的 Commit 歷史紀錄
- Pre-commit Hooks 執行失敗

## 替代方案

若使用者希望自行控制，請建議：
1. **選擇性暫存**：檢查指定檔案並加入暫存區
2. **互動式暫存**：以 `git add -p` 逐段挑選
3. **PR 工作流程**：建立分支 → Push → PR（使用 `/pr` 指令）

**⚠️ 請記住**：Push 前一定要檢查變更。有疑慮時，逐一使用 Git 指令，以便更精確控制。

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
