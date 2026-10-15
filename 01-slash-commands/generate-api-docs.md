---
description: 從原始程式碼產生完整的 API 文件
---

# API 文件產生工具

依照以下步驟產生 API 文件：

1. 掃描 `/src/api/` 內的所有檔案
2. 擷取函式簽章和 JSDoc 註解
3. 依端點／模組整理
4. 以 Markdown 建立文件與範例
5. 包含請求／回應的結構描述
6. 加入錯誤處理文件

輸出格式：
- 產生 `/docs/api.md` Markdown 檔案
- 為所有端點加入 curl 範例
- 加入 TypeScript 型別

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/commands
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
