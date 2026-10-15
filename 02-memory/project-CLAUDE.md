# 專案設定

## 專案概述
- **名稱**：電子商務平台
- **技術組合**：Node.js、PostgreSQL、React 18、Docker
- **團隊規模**：5 位開發者
- **截止期限**：2025 年第 4 季

## 架構
@docs/architecture.md
@docs/api-standards.md
@docs/database-schema.md

## 開發規範

### 程式碼風格
- 使用 Prettier 格式化程式碼
- 使用 ESLint 搭配 Airbnb 設定
- 每行最長 100 個字元
- 使用 2 個空白字元縮排

### 命名慣例
- **檔案**：kebab-case（user-controller.js）
- **類別**：PascalCase（UserService）
- **函式／變數**：camelCase（getUserById）
- **常數**：UPPER_SNAKE_CASE（API_BASE_URL）
- **資料表**：snake_case（user_accounts）

### Git 工作流程
- 分支名稱：`feature/description` 或 `fix/description`
- Commit 訊息：遵循 Conventional Commits 規範
- Merge 前必須先建立 PR
- 所有 CI/CD 檢查皆須通過
- 至少取得 1 人核准

### 測試要求
- 程式碼涵蓋率至少 80%
- 所有關鍵流程都必須有測試
- 單元測試使用 Jest
- 端對端（E2E）測試使用 Cypress
- 測試檔案命名：`*.test.ts` 或 `*.spec.ts`

### API 規範
- 僅使用 RESTful 端點
- 請求／回應使用 JSON
- 正確使用 HTTP 狀態碼
- API 端點加入版本號：`/api/v1/`
- 所有端點都必須附範例文件

### 資料庫
- 使用 Migration 修改資料結構
- 絕不將憑證寫死於程式碼
- 使用連線池
- 在開發環境啟用查詢日誌
- 定期備份

### 部署
- 使用 Docker 部署
- 使用 Kubernetes 編排
- 採用藍綠部署策略
- 失敗時自動回復
- 部署前先執行資料庫 Migration

## 常用指令

| 指令 | 用途 |
|------|------|
| `npm run dev` | 啟動開發伺服器 |
| `npm test` | 執行測試套件 |
| `npm run lint` | 檢查程式碼風格 |
| `npm run build` | 建置正式環境版本 |
| `npm run migrate` | 執行資料庫 Migration |

## 團隊聯絡人
- 技術主管：Sarah Chen（@sarah.chen）
- 產品經理：Mike Johnson（@mike.j）
- DevOps：Alex Kim（@alex.k）

## 已知問題與因應方式
- PostgreSQL 連線池在尖峰時段限制為 20 條連線
- 因應方式：實作查詢佇列
- Safari 14 與非同步產生器有相容性問題
- 因應方式：使用 Babel 轉譯器

## 相關專案
- 分析儀表板：`/projects/analytics`
- 行動應用程式：`/projects/mobile`
- 管理後台：`/projects/admin`

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/memory
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
