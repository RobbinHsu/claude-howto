---
allowed-tools: Bash(git add:*), Bash(git status:*), Bash(git commit:*), Bash(git diff:*)
argument-hint: [message]
description: 根據目前修改內容建立 Git Commit
---

## 上下文

- 目前 Git 狀態：!`git status`
- 目前 Git 差異：!`git diff HEAD`
- 目前分支：!`git branch --show-current`
- 最近的 Commit：!`git log --oneline -10`

## 你的任務

根據上述修改，建立單一 Git Commit。

若透過參數提供訊息，則使用該訊息：$ARGUMENTS

否則，請分析變更並依照 Conventional Commits 格式產生適當的 Commit 訊息：
- `feat:` 表示新增功能
- `fix:` 表示修正錯誤
- `docs:` 表示文件變更
- `refactor:` 表示程式碼重構
- `test:` 表示新增測試
- `chore:` 表示維護工作

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
