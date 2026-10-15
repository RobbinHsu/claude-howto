---
description: 整理程式碼、暫存變更並準備 Pull Request
allowed-tools: Bash(git add:*), Bash(git status:*), Bash(git diff:*), Bash(npm test:*), Bash(npm run lint:*)
---

# Pull Request 準備檢查清單

建立 PR 之前，請執行以下步驟：

1. 執行程式碼檢查：`prettier --write .`
2. 執行測試：`npm test`
3. 檢視 Git 差異：`git diff HEAD`
4. 將變更加入暫存區：`git add .`
5. 依 Conventional Commits 規範建立 Commit 訊息：
   - `fix:` 修正錯誤
   - `feat:` 新增功能
   - `docs:` 文件變更
   - `refactor:` 重整程式碼結構
   - `test:` 新增測試
   - `chore:` 維護工作

6. 產生 PR 摘要，包含：
   - 修改了什麼
   - 為什麼需要修改
   - 執行了哪些測試
   - 潛在影響

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
