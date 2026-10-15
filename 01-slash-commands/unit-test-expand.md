---
name: unit-test-expand
description: 針對尚未測試的分支及邊界情況，提高測試涵蓋率
---

# 擴充單元測試

依照專案使用的測試框架，擴充現有單元測試：

1. **分析涵蓋率**：執行涵蓋率報告，找出尚未測試的分支、邊界情況及低涵蓋率區域
2. **找出缺口**：檢查程式碼的邏輯分支、錯誤處理路徑、邊界條件，以及 null／空白輸入
3. **使用專案現有框架撰寫測試**：
   - Jest／Vitest／Mocha（JavaScript／TypeScript）
   - pytest／unittest（Python）
   - Go testing／testify（Go）
   - Rust 測試框架（Rust）
4. **針對特定情境**：
   - 錯誤處理與例外狀況
   - 邊界值（最小／最大、空值、null）
   - 特殊與極端情況
   - 狀態轉換與副作用
5. **驗證改善成果**：重新執行涵蓋率測試，確認數值有明確提升

只呈現新增的測試程式碼區塊。遵循現有測試模式與命名慣例。

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
