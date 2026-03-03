# 台灣微網科技 - 開發程序標準作業程序

## 📋 概述

本文檔詳述台灣微網科技股份有限公司（TMC）軟體開發之標準作業程序（SOP），確保開發流程標準化、程式碼品質一致性を維持。

---

## 🏢 開發架構

### 技術堆疊

| 類別 | 技術 |
|------|------|
| 前端框架 | React, Next.js |
| 後端框架 | Node.js, Express |
| 資料庫 | PostgreSQL, MongoDB |
| 雲端平台 | Vercel, AWS |
| 版控 | Git, GitHub |
| 專案管理 | Notion |

### 開發環境

- **Node.js 版本**: 20.x LTS
- **瀏覽器支援**: Chrome, Firefox, Safari, Edge (最新 2 版本)
- **IDE**: VS Code (推薦)

---

## 📝 開發流程

### 1. 需求確認

- 從 Notion 任務資料庫取得需求
- 與產品經理確認功能規格
- 評估開發時程

### 2. 環境設定

```bash
# Clone 專案
git clone https://github.com/tingkuanli91-source/[project-name].git

# 安裝依賴
npm install

# 啟動開發伺服器
npm run dev
```

### 3. 程式碼規範

- 使用 ESLint + Prettier 進行程式碼格式化
- 遵循 React 最佳實踐
- 使用 TypeScript (建議)
- 提交前必須通過 lint 檢查

### 4. 版本控制

- 使用 Git Flow 分支策略
- `main` - 生產環境
- `develop` - 開發環境
- `feature/*` - 功能分支
- `bugfix/*` - 錯誤修復

### 5. 提交規範

```
feat: 新功能
fix: 錯誤修復
docs: 文件更新
style: 程式碼格式
refactor: 重構
test: 測試
chore: 建置/工具
```

---

## 🚀 部署流程

### Vercel 部署

1. 推送程式碼至 GitHub
2. Vercel 自動觸發部署
3. 檢視部署狀態
4. 確認上線

### Docker 部署

```bash
# 構建映像
docker build -t [image-name]:[tag] .

# 執行容器
docker run -p 3000:3000 [image-name]:[tag]
```

---

## ✅ 品質保證

### 程式碼審查

- 提交 Pull Request
- 至少一人 Code Review
- 通過自動化測試

### 測試策略

- 單元測試 (Jest)
- 整合測試
- E2E 測試 (Cypress)

---

## 📊 已開發專案清單

| 專案名稱 | 網址 | 說明 |
|----------|------|------|
| Factory Power Management | factory-pwr-sys.vercel.app | 工廠用電管理系統 |
| Factory Power Management v3 | factory-power-v3.vercel.app | 操作者版本 |
| Factory Power Flow | factory-pwr.vercel.app | 功率流向圖 |
| Microgrid Dashboard | microgrid-dashboard.vercel.app | 微網案例儀表板 |
| Taiwan Microgrid O&M | taiwan-microgrid-om.vercel.app | 維運系統 |
| Energy Mobile EMS | energy-mobile.vercel.app | 手機版能源管理 |
| Pomodoro Timer | pomodoro-timer.vercel.app | 番茄鐘 |
| Type Keyboard | type-keyboard.vercel.app | 打字練習 |

---

## 📞 聯繫資訊

- **公司**: 台灣微網科技股份有限公司
- **Email**: admin@taiwanmicrogrid.com

---

*最後更新: 2026-03-03*
