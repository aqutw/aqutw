# aqutw

Go 後端、Web 與 Mobile、LLM 應用的實作紀錄。

## 2026 公開專案

依 repository 建立時間由新到舊排列，收錄至 `go-api`。每個專案附功能簡介與主要技術標籤。

| 專案 | 簡介 | 技術棧 |
| --- | --- | --- |
| [typescript-202610](https://github.com/aqutw/typescript-202610) | 120 個可執行的 TypeScript 範例，依初、中、高階各分 40 題；涵蓋型別收斂、泛型、狀態機與非同步控制，附對應 JavaScript 與斷言驗證。 | `TypeScript` `JavaScript` `Node.js` |
| [Pydantic-demo](https://github.com/aqutw/Pydantic-demo) | 以使用者與訂單模型示範 Pydantic v2 的巢狀驗證、strict mode、自訂驗證、Decimal 序列化及 JSON Schema 匯出，附 CLI、單元測試與 CI。 | `Python` `Pydantic v2` `JSON Schema` `unittest` `GitHub Actions` |
| [JSON-Schema-demo](https://github.com/aqutw/JSON-Schema-demo) | 以 JSON Schema Draft 2020-12 與 Ajv 示範使用者、付款資料契約；涵蓋巢狀參照、條件與 oneOf 驗證，附 CLI、有效／無效案例及測試。 | `JavaScript` `Node.js` `JSON Schema` `Ajv` `GitHub Actions` |
| [extract-ChatGPT-chat-time](https://github.com/aqutw/extract-ChatGPT-chat-time) | 掃描 ChatGPT 匯出的 conversations-*.json，逐檔列出對話數、最早建立與最晚更新時間；支援時區設定並輸出 TSV，無第三方依賴。 | `JavaScript` `Node.js` `JSON` `TSV` |
| [jobLineBot](https://github.com/aqutw/jobLineBot) | 擷取並清理 104 職缺，透過 OpenRouter 產生職缺分析與六題模擬面試，再由 LINE 非同步推播；另提供支援六個求職網站的瀏覽器快照分析 API。 | `Go` `net/http` `OpenRouter` `LINE Messaging API` `Render` `GitHub Actions` |
| [lineAtBot](https://github.com/aqutw/lineAtBot) | LINE 台股歷史行情問答：由 LLM 透過工具呼叫產生唯讀 SQL，查詢匯入的 OHLC 與股票分類資料，再依結果回答；可使用 SQLite 或 PostgreSQL。 | `Go` `OpenRouter` `LINE Messaging API` `SQL` `SQLite` `PostgreSQL` `Render` |
| [Golang-with-Gin-ecommerce-API-starter-202610](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610) | 以 go.work 組織 commerce、identity、platform 與 API 的模組化單體；實作優惠策略、庫存與冪等結帳，以及 JWT、refresh token 輪替及 session 撤銷。 | `Go` `Gin` `SQLite` `JWT` `Argon2id` `Docker` `GitHub Actions` |
| [microservice-bff-api](https://github.com/aqutw/microservice-bff-api) | 電商微服務 PoC：Next.js 商店串接獨立 Web／App BFF 與 Go 訂單、庫存、模擬付款、稽核服務；實作持久化 Saga、冪等補償與 OIDC 登入，附故障恢復整合測試及 k6 壓測。 | `Go` `Node.js` `Next.js` `React` `SQLite` `Keycloak` `OIDC` `Docker Compose` `Kubernetes` `k6` `GitHub Actions` |
| [auto-job-site](https://github.com/aqutw/auto-job-site) | 共用 SQLite 職缺資料的跨平台看板 PoC：Go／Gin 或 NestJS 提供可替換 API，搭配 Next.js、Nuxt 與 Expo React Native，支援多關鍵字搜尋與職缺詳情。 | `Go` `Gin` `TypeScript` `NestJS` `Next.js` `Nuxt` `Vue` `React Native` `Expo` `SQLite` `Tailwind CSS` `Docker` `GitHub Actions` |
| [go-api](https://github.com/aqutw/go-api) | Go／Gin GitOps 練習，提供 health、version、示範 users 與 Prometheus metrics；附 GHCR 映像建置流程，以及 Kubernetes、Kustomize、Argo CD 與 Image Updater 設定範例。 | `Go` `Gin` `Prometheus` `Docker` `GHCR` `Kubernetes` `Kustomize` `Argo CD` `GitHub Actions` |

內容核對於 **2026-10-20**，依各 repo 的原始碼與 commit 歷史整理。[查看檔案與變更依據](docs/project-evidence-2026.md)。
