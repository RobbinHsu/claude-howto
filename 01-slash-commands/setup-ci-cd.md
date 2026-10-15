---
name: setup-ci-cd
description: 建立 Pre-commit Hooks 和 GitHub Actions，以確保程式碼品質
---

# 設定 CI/CD 流程

根據專案類型建立完整的 DevOps 品質關卡：

1. **分析專案**：偵測使用的程式語言、框架、建置系統及現有工具
2. **設定 Pre-commit Hooks**，搭配適合該語言的工具：
   - 格式化：Prettier／Black／gofmt／rustfmt 等
   - 程式碼檢查：ESLint／Ruff／golangci-lint／Clippy 等
   - 安全性：Bandit／gosec／cargo-audit／npm audit 等
   - 型別檢查：TypeScript／mypy／flow（若適用）
   - 測試：執行相關測試套件
3. **建立 GitHub Actions 工作流程**（`.github/workflows/`）：
   - 在 Push／PR 時執行與 Pre-commit 相同的檢查
   - 多版本／多平台測試矩陣（若適用）
   - 建置與測試驗證
   - 部署步驟（若需要）
4. **驗證流程**：在本機測試、建立測試 PR，確認所有檢查皆通過

使用免費／開放原始碼工具。尊重現有設定，並保持快速執行。

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
