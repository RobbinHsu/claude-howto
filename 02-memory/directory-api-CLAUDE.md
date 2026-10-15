# API 模組規範

本檔案補充根目錄 CLAUDE.md 中適用於 `/src/api/` 下所有內容的規則。記憶檔案會合併串接，而不是彼此覆蓋——根目錄的 CLAUDE.md 仍然有效；當 Claude Code 讀取、寫入或編輯這個子目錄的檔案時，會視需要載入本檔案。

## API 專用規範

### 請求驗證
- 使用 Zod 驗證資料結構
- 一律驗證輸入資料
- 驗證失敗時傳回 400 與錯誤資訊
- 包含欄位層級的錯誤詳細資訊

### 身分驗證
- 所有端點皆要求 JWT Token
- Token 放在 Authorization 標頭
- Token 在 24 小時後過期
- 實作 Refresh Token 機制

### 回應格式

所有回應都必須符合以下結構：

```json
{
  "success": true,
  "data": { /* 實際資料 */ },
  "timestamp": "2025-11-06T10:30:00Z",
  "version": "1.0"
}
```

錯誤回應：
```json
{
  "success": false,
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "使用者可讀的訊息",
    "details": { /* 欄位錯誤 */ }
  },
  "timestamp": "2025-11-06T10:30:00Z"
}
```

### 分頁
- 使用游標式分頁（不要使用 Offset）
- 包含 `hasMore` 布林值
- 每頁上限為 100 筆
- 預設每頁 20 筆

### 速率限制
- 已驗證的使用者每小時最多 1,000 次請求
- 公開端點每小時最多 100 次請求
- 超過限制時傳回 429
- 包含 retry-after 標頭

### 快取
- 使用 Redis 儲存工作階段快取
- 預設快取時間為 5 分鐘
- 寫入操作時使快取失效
- 在快取鍵上標記資源類型

---
**最後更新日期**：2026 年 10 月 10 日
**Claude Code 版本**：2.1.296
**資料來源**：
- https://code.claude.com/docs/en/memory
- https://github.com/anthropics/claude-code/releases/tag/v2.1.288
- https://github.com/anthropics/claude-code/releases/tag/v2.1.293
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
