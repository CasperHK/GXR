# GXR Stack (Goravel + React Router[Remix] + Radix)
GXR 是一個為 2026 年 Web 開發設計的高性能全棧框架。它完美的結合了 Golang 的企業級後端效能、Remix 的先進伺服器端渲染（SSR）技術，以及 Radix UI 無障礙設計的底層元件庫。


## 🚀 技術棧組成
* [G] **[Goravel](https://www.goravel.dev/)**: 基於 Go 語言的高生產力開發框架。受 Laravel 啟發，提供強大的 ORM、資料遷移（Migration）、認證與任務排程，並保有編譯型語言的極致速度。
* [X] **[Remix (React Router 7+)](https://remix.run/)**: 現代前端路由引擎。利用 Web 標準與巢狀路由（Nested Routes），徹底消除加載狀態（Loading States）並提供卓越的 SEO 表現。
* [R] **[Radix UI](https://www.radix-ui.com/)**: 開源的無標題（Headless）UI 元件庫。專注於處理複雜的無障礙訪問（WAI-ARIA）與鍵盤操作邏輯，讓你擁有 100% 的樣式掌控權。

## ✨ 核心優勢
* 極致效能：利用 Goravel 的 Go 核心確保微秒級的 API 回應時間，結合 Remix 的邊緣運算（Edge-ready）運行環境，大幅提升加載速度。
* 類型安全通信：透過定義共享的 Schema，縮短 Go 後端模型與 Remix Loader 之間的「數據落差」。
* 無障礙優先：所有基於 Radix 的 UI 元件原生支援螢幕閱讀器與鍵盤導覽，符合現代 Web 標準。
* 統一的開發體驗 (DX)：呼應 2026 年流行的「意圖導向編碼 (Intent-based Coding)」，GXR 提供了直觀的 CLI 工具與 AI 輔助的開發模板。

---

## 🛠️ 快速上手
### 前置準備
* [Go](https://go.dev/) 1.22+
* [Node.js](https://nodejs.org/en) 20+
* Goravel CLI

### 安裝步驟
複製專案範本：
```bash
git clone https://github.com
cd gxr-stack
```

### 啟動 Goravel 後端：
```bash
cd backend
cp .env.example .env
go mod download
go run . migrate
```

啟動 Remix 前端：
```bash
cd ../frontend
npm install
npm run dev
```

## 📂 專案結構
```text
/src
 ├── backend/            # Goravel (Go) - API, ORM, 任務調度
 │   ├── app/            # 業務邏輯與控制器
 │   ├── routes/         # API 路由定義
 │   └── database/       # 資料庫遷移與數據填充
 ├── frontend/           # Remix (TS) - UI, 路由, Loader
 │   ├── app/            # Remix 路由與頁面
 │   └── components/     # 基於 Radix 的 UI 底層組件
 └── docker-compose.yml  # 本地開發環境配置
```

## 📜 授權協議
GXR 是一款基於 MIT 授權協議 的開源軟體。
