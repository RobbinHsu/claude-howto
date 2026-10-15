# 我的開發偏好

## 關於我
- **經驗程度**：8 年全端開發經驗
- **偏好的語言**：TypeScript、Python
- **溝通風格**：直接，並附帶範例
- **學習方式**：結合程式碼的視覺化圖表

## 程式碼偏好

### 錯誤處理
我偏好使用 try-catch 區塊進行明確的錯誤處理，並提供有意義的錯誤訊息。
避免模糊籠統的錯誤。務必記錄錯誤以利除錯。

### 註解
註解應解釋「為什麼」，而不是「做了什麼」。程式碼本身應該清楚表達意圖。
註解應說明商業邏輯或不易理解的決策。

### 測試
我偏好 TDD（測試驅動開發）。
先撰寫測試，再實作功能。
重點放在行為，而非實作細節。

### 架構
我偏好模組化、低耦合的設計。
使用相依性注入以提升可測試性。
做好關注點分離（Controllers、Services、Repositories）。

## 除錯偏好
- 使用 `console.log` 並加上 `[DEBUG]` 前綴
- 包含上下文：函式名稱與相關變數
- 可以取得時，附上堆疊追蹤資訊
- 日誌務必包含時間戳記

## 溝通方式
- 利用圖表解釋複雜概念
- 先展示具體範例，再說明理論
- 提供修改前／後的程式碼片段
- 在最後整理重點

## 專案組織
我的專案目錄通常如下：
```
project/
  ├── src/
  │   ├── api/
  │   ├── services/
  │   ├── models/
  │   └── utils/
  ├── tests/
  ├── docs/
  └── docker/
```

## 工具
- **IDE**：VS Code 搭配 Vim 快捷鍵
- **終端機**：Zsh 搭配 Oh-My-Zsh
- **格式化**：Prettier（每行最多 100 個字元）
- **程式碼檢查**：ESLint 搭配 Airbnb 設定
- **測試框架**：Jest 搭配 React Testing Library

---
**最後更新日期**：2026 年 8 月 4 日
**Claude Code 版本**：2.1.220
**資料來源**：
- https://code.claude.com/docs/en/memory
**相容模型**：Claude Fable 5、Claude Opus 5、Claude Sonnet 5、Claude Sonnet 4.6、Claude Opus 4.8、Claude Haiku 4.5
