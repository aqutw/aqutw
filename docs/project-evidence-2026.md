# 2026 專案內容核對紀錄

核對日期：2026-10-20（Asia/Taipei）。

範圍：aqutw 在 2026 年建立的公開 repositories，依建立時間由新到舊，包含 go-api，共 10 個。Profile repo 本身不列入專案清單。

簡介與標籤依預設分支的程式檔案、依賴設定、測試及 commit 歷史交叉核對。下列檔案連結固定到本次檢查的 commit；紀錄反映靜態閱讀結果。

## typescript-202610

120 個可執行的 TypeScript 範例，依初、中、高階各分 40 題；涵蓋型別收斂、泛型、狀態機與非同步控制，附對應 JavaScript 與斷言驗證。

主要技術：`TypeScript` `JavaScript` `Node.js`。

檢查版本：[`d211a15`](https://github.com/aqutw/typescript-202610/commit/d211a1581fba14c894c1c9ab51e2087d0d279330)。

檔案依據：

- [`package.json`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/package.json)
- [`tsconfig.json`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/tsconfig.json)
- [`scripts/verify-examples.mjs`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/scripts/verify-examples.mjs)
- [`easy/22-discriminated-unions.ts`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/easy/22-discriminated-unions.ts)
- [`hard/03-exhaustive-state-machine.ts`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/hard/03-exhaustive-state-machine.ts)
- [`hard/19-bounded-async-concurrency.ts`](https://github.com/aqutw/typescript-202610/blob/d211a1581fba14c894c1c9ab51e2087d0d279330/hard/19-bounded-async-concurrency.ts)

變更依據：

- [`d211a15`](https://github.com/aqutw/typescript-202610/commit/d211a1581fba14c894c1c9ab51e2087d0d279330)：Add 120 runnable TypeScript examples across three difficulty levels

範圍說明：原始碼與驗證腳本均定義三個難度、每組 40 題，並檢查編譯後 JavaScript 與提交版本一致。此 repo 刻意未放 README，簡介依程式與首筆 commit 撰寫。

## Pydantic-demo

以使用者與訂單模型示範 Pydantic v2 的巢狀驗證、strict mode、自訂驗證、Decimal 序列化及 JSON Schema 匯出，附 CLI、單元測試與 CI。

主要技術：`Python` `Pydantic v2` `JSON Schema` `unittest` `GitHub Actions`。

檢查版本：[`6684c29`](https://github.com/aqutw/Pydantic-demo/commit/6684c29e7ebe7ef3d6b606688b30ae628c57b713)。

檔案依據：

- [`pyproject.toml`](https://github.com/aqutw/Pydantic-demo/blob/6684c29e7ebe7ef3d6b606688b30ae628c57b713/pyproject.toml)
- [`src/pydantic_demo/models.py`](https://github.com/aqutw/Pydantic-demo/blob/6684c29e7ebe7ef3d6b606688b30ae628c57b713/src/pydantic_demo/models.py)
- [`src/pydantic_demo/__main__.py`](https://github.com/aqutw/Pydantic-demo/blob/6684c29e7ebe7ef3d6b606688b30ae628c57b713/src/pydantic_demo/__main__.py)
- [`tests/test_models.py`](https://github.com/aqutw/Pydantic-demo/blob/6684c29e7ebe7ef3d6b606688b30ae628c57b713/tests/test_models.py)
- [`.github/workflows/ci.yml`](https://github.com/aqutw/Pydantic-demo/blob/6684c29e7ebe7ef3d6b606688b30ae628c57b713/.github/workflows/ci.yml)

變更依據：

- [`6684c29`](https://github.com/aqutw/Pydantic-demo/commit/6684c29e7ebe7ef3d6b606688b30ae628c57b713)：Add Pydantic v2 validation and serialization demos

範圍說明：模型中的 computed_field 計算訂單總額，TypeAdapter 處理付款方式辨別聯集；CLI 支援 demo、validate、schema。付款資料僅為驗證範例。

## JSON-Schema-demo

以 JSON Schema Draft 2020-12 與 Ajv 示範使用者、付款資料契約；涵蓋巢狀參照、條件與 oneOf 驗證，附 CLI、有效／無效案例及測試。

主要技術：`JavaScript` `Node.js` `JSON Schema` `Ajv` `GitHub Actions`。

檢查版本：[`7aec542`](https://github.com/aqutw/JSON-Schema-demo/commit/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f)。

檔案依據：

- [`package.json`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/package.json)
- [`schemas/user.schema.json`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/schemas/user.schema.json)
- [`schemas/payment.schema.json`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/schemas/payment.schema.json)
- [`src/validator.js`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/src/validator.js)
- [`src/cli.js`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/src/cli.js)
- [`test/validator.test.js`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/test/validator.test.js)
- [`.github/workflows/ci.yml`](https://github.com/aqutw/JSON-Schema-demo/blob/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f/.github/workflows/ci.yml)

變更依據：

- [`7aec542`](https://github.com/aqutw/JSON-Schema-demo/commit/7aec542dfa2ea9df0a173efd6fc0041a8fbd450f)：Add runnable JSON Schema validation demos with Ajv

範圍說明：Ajv 使用 Draft 2020-12、strict 與 allErrors，另載入 ajv-formats；不做型別轉換、不插入預設值、不移除未知欄位。付款 schema 並非金流整合。

## extract-ChatGPT-chat-time

掃描 ChatGPT 匯出的 conversations-*.json，逐檔列出對話數、最早建立與最晚更新時間；支援時區設定並輸出 TSV，無第三方依賴。

主要技術：`JavaScript` `Node.js` `JSON` `TSV`。

檢查版本：[`aa22bee`](https://github.com/aqutw/extract-ChatGPT-chat-time/commit/aa22bee95ae9caaacf93f025b3a8a4cf4fef38fe)。

檔案依據：

- [`README.md`](https://github.com/aqutw/extract-ChatGPT-chat-time/blob/aa22bee95ae9caaacf93f025b3a8a4cf4fef38fe/README.md)
- [`list-conversation-dates.js`](https://github.com/aqutw/extract-ChatGPT-chat-time/blob/aa22bee95ae9caaacf93f025b3a8a4cf4fef38fe/list-conversation-dates.js)

變更依據：

- [`aa22bee`](https://github.com/aqutw/extract-ChatGPT-chat-time/commit/aa22bee95ae9caaacf93f025b3a8a4cf4fef38fe)：init

範圍說明：工具統計每個檔案內的對話數，而非訊息數。時間取 create_time 與 update_time，更新時間無效時回退至建立時間；透過 TZ 選擇本機時區。

## jobLineBot

擷取並清理 104 職缺，透過 OpenRouter 產生職缺分析與六題模擬面試，再由 LINE 非同步推播；另提供支援六個求職網站的瀏覽器快照分析 API。

主要技術：`Go` `net/http` `OpenRouter` `LINE Messaging API` `Render` `GitHub Actions`。

檢查版本：[`55e6e9d`](https://github.com/aqutw/jobLineBot/commit/55e6e9d6f92f6e147448450da0363c70994698f8)。

檔案依據：

- [`go.mod`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/go.mod)
- [`internal/bot/service.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/bot/service.go)
- [`internal/job104/job.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/job104/job.go)
- [`internal/web/server.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/web/server.go)
- [`internal/web/extension.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/web/extension.go)
- [`internal/web/sites.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/web/sites.go)
- [`internal/line/client.go`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/internal/line/client.go)
- [`render.yaml`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/render.yaml)
- [`.github/workflows/ci.yml`](https://github.com/aqutw/jobLineBot/blob/55e6e9d6f92f6e147448450da0363c70994698f8/.github/workflows/ci.yml)

變更依據：

- [`ad98bf1`](https://github.com/aqutw/jobLineBot/commit/ad98bf1bd5f661894cbeaa40885a73084135d60a)：Build 104 job analysis LINE bot with Go retrieval and OpenRouter
- [`4d6ad0a`](https://github.com/aqutw/jobLineBot/commit/4d6ad0addfa9631a94e6d42decc8337ca89be21e)：Deliver slow free-model analyses through LINE push messages
- [`15cb8e7`](https://github.com/aqutw/jobLineBot/commit/15cb8e7233a05f68fd4d92c9d1cd85e14452b9c3)：Add anonymous snapshot analysis endpoint for Chrome extension
- [`55e6e9d`](https://github.com/aqutw/jobLineBot/commit/55e6e9d6f92f6e147448450da0363c70994698f8)：Support six job sites in shared snapshot analysis API

範圍說明：六站為 104、Cake、Yourator、1111、yes123、518，僅快照 API 支援此範圍。LINE 與受保護的網址抓取入口仍使用 104 擷取器；repo 內沒有 Chrome 擴充功能前端。Render Blueprint 與 CI 為 repo 內設定，未據此推定線上服務可用。

## lineAtBot

LINE 台股歷史行情問答：由 LLM 透過工具呼叫產生唯讀 SQL，查詢匯入的 OHLC 與股票分類資料，再依結果回答；可使用 SQLite 或 PostgreSQL。

主要技術：`Go` `OpenRouter` `LINE Messaging API` `SQL` `SQLite` `PostgreSQL` `Render`。

檢查版本：[`b776639`](https://github.com/aqutw/lineAtBot/commit/b776639d9fbaf0008350fbc312eb63514c980131)。

檔案依據：

- [`go.mod`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/go.mod)
- [`internal/bot/service.go`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/internal/bot/service.go)
- [`internal/openrouter/client.go`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/internal/openrouter/client.go)
- [`internal/stock/sql.go`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/internal/stock/sql.go)
- [`internal/stock/store.go`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/internal/stock/store.go)
- [`internal/stock/sql_test.go`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/internal/stock/sql_test.go)
- [`scripts/import_wantg.py`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/scripts/import_wantg.py)
- [`migrations/001_postgres.sql`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/migrations/001_postgres.sql)
- [`render.yaml`](https://github.com/aqutw/lineAtBot/blob/b776639d9fbaf0008350fbc312eb63514c980131/render.yaml)

變更依據：

- [`1161942`](https://github.com/aqutw/lineAtBot/commit/1161942e6038aca31fec4047289dec9837e9d9a8)：Replace demo prices with user-provided historical OHLC dataset
- [`58fe660`](https://github.com/aqutw/lineAtBot/commit/58fe6602634e313ebade17c88b05b479a026bf7b)：Let LLM query OHLC data and write unrestricted natural replies
- [`2bf53ad`](https://github.com/aqutw/lineAtBot/commit/2bf53addbe6d3bac2c76d1638dcccfaa9cd704dd)：Specify the reply when a requested stock is absent
- [`79e6a7a`](https://github.com/aqutw/lineAtBot/commit/79e6a7ad475a8f6fd5867b7c5f6d55593ab68070)：Explain reported model failures with safe diagnostics

範圍說明：資料來自匯入的歷史 CSV。SQLite 使用 authorizer 與唯讀連線；PostgreSQL 使用唯讀 transaction。兩者都有查詢時間與結果大小限制。簡介不將資料描述為即時行情，也不保證模型永不出錯。

## Golang-with-Gin-ecommerce-API-starter-202610

以 go.work 組織 commerce、identity、platform 與 API 的模組化單體；實作優惠策略、庫存與冪等結帳，以及 JWT、refresh token 輪替及 session 撤銷。

主要技術：`Go` `Gin` `SQLite` `JWT` `Argon2id` `Docker` `GitHub Actions`。

檢查版本：[`c35b477`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/commit/c35b4774185c97043ef33a313c371d0f4f9c8636)。

檔案依據：

- [`go.work`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/go.work)
- [`apps/api/go.mod`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/apps/api/go.mod)
- [`apps/api/internal/httpapi/router.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/apps/api/internal/httpapi/router.go)
- [`modules/commerce/application/checkout/service.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/commerce/application/checkout/service.go)
- [`modules/commerce/domain/discount/strategy.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/commerce/domain/discount/strategy.go)
- [`modules/commerce/adapters/sqlite/store.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/commerce/adapters/sqlite/store.go)
- [`modules/identity/application/service.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/identity/application/service.go)
- [`modules/identity/adapters/secure/jwt.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/identity/adapters/secure/jwt.go)
- [`modules/identity/adapters/secure/password.go`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/modules/identity/adapters/secure/password.go)
- [`Dockerfile`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/Dockerfile)
- [`.github/workflows/ci-cd.yml`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/blob/c35b4774185c97043ef33a313c371d0f4f9c8636/.github/workflows/ci-cd.yml)

變更依據：

- [`4a8952b`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/commit/4a8952b16edd7c79df941c30297dc4705488ede8)：init starter
- [`5877580`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/commit/58775805ac07fccbe54a7cf571b8f6fe0ea87604)：feat: add discount logic
- [`3844086`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/commit/3844086e274c7f1052a2b33f173b8aeca594d224)：feat: complete JWT + Refresh Token
- [`b47f852`](https://github.com/aqutw/Golang-with-Gin-ecommerce-API-starter-202610/commit/b47f8527dfb98b58830877e19cc0910fe668420c)：fix(deps): synchronize API lockfiles with identity crypto upgrade

範圍說明：此為單一 API process 的四模組 starter。訂單停在 pending_payment，尚未整合實際付款、庫存保留到期處理與 outbox 發送 worker；不得與下方電商微服務 PoC 混稱。

## microservice-bff-api

電商微服務 PoC：Next.js 商店串接獨立 Web／App BFF 與 Go 訂單、庫存、模擬付款、稽核服務；實作持久化 Saga、冪等補償與 OIDC 登入，附故障恢復整合測試及 k6 壓測。

主要技術：`Go` `Node.js` `Next.js` `React` `SQLite` `Keycloak` `OIDC` `Docker Compose` `Kubernetes` `k6` `GitHub Actions`。

檢查版本：[`9672af7`](https://github.com/aqutw/microservice-bff-api/commit/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec)。

檔案依據：

- [`website/package.json`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/website/package.json)
- [`website/lib/auth.mjs`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/website/lib/auth.mjs)
- [`bff-api/package.json`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/bff-api/package.json)
- [`bff-api/src/desktop.js`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/bff-api/src/desktop.js)
- [`bff-api/src/app.js`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/bff-api/src/app.js)
- [`services/order/go.mod`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/services/order/go.mod)
- [`services/order/saga.go`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/services/order/saga.go)
- [`services/order/settlement.go`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/services/order/settlement.go)
- [`services/payment/main.go`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/services/payment/main.go)
- [`services/audit-worker/main.go`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/services/audit-worker/main.go)
- [`docker-compose.dev.yml`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/docker-compose.dev.yml)
- [`k8s/poc.yaml`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/k8s/poc.yaml)
- [`loadtest/commerce.js`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/loadtest/commerce.js)
- [`scripts/settlement-sit.mjs`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/scripts/settlement-sit.mjs)
- [`.github/workflows/sit.yml`](https://github.com/aqutw/microservice-bff-api/blob/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec/.github/workflows/sit.yml)

變更依據：

- [`bb9f4fb`](https://github.com/aqutw/microservice-bff-api/commit/bb9f4fb3cb2bbfe187e1ecb0bd159c7e49f52945)：feat(checkout): persist saga progress and recovery jobs
- [`1e2ba6f`](https://github.com/aqutw/microservice-bff-api/commit/1e2ba6f4abc32dfdb4831affc97580a130d85898)：feat(security): enforce identity and resource access
- [`4e1ad2d`](https://github.com/aqutw/microservice-bff-api/commit/4e1ad2dab26679b457335f55cfc03b789c6bd747)：feat(order): coordinate durable settlement through one BFF entry point
- [`cc32de2`](https://github.com/aqutw/microservice-bff-api/commit/cc32de28e49a5d5fcf72b121794061948b704055)：fix(order): coordinate cancellation with settlement and payment compensation
- [`a2ee740`](https://github.com/aqutw/microservice-bff-api/commit/a2ee740e5ed91feb6ead1c26d861463b92d6a64e)：test(sit): recover in-flight crashes and fence stale workers after lease expiry
- [`9672af7`](https://github.com/aqutw/microservice-bff-api/commit/9672af7080bd0b7311f5bfda0e2b5def57e8e9ec)：ci(coverage): publish Go race and Node unit coverage reports

範圍說明：目前 BFF 是 Node.js HTTP server，不能因 repo 名稱或生態系推斷為 Express。付款與退款為模擬流程；SQLite 服務仍採單副本。Kubernetes manifest 與壓測腳本的存在不代表已在正式叢集部署或達到特定效能數字。

## auto-job-site

共用 SQLite 職缺資料的跨平台看板 PoC：Go／Gin 或 NestJS 提供可替換 API，搭配 Next.js、Nuxt 與 Expo React Native，支援多關鍵字搜尋與職缺詳情。

主要技術：`Go` `Gin` `TypeScript` `NestJS` `Next.js` `Nuxt` `Vue` `React Native` `Expo` `SQLite` `Tailwind CSS` `Docker` `GitHub Actions`。

檢查版本：[`f09621f`](https://github.com/aqutw/auto-job-site/commit/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e)。

檔案依據：

- [`api-golang/go.mod`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/api-golang/go.mod)
- [`api-golang/server.go`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/api-golang/server.go)
- [`api-golang/search.go`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/api-golang/search.go)
- [`api-nestjs/package.json`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/api-nestjs/package.json)
- [`api-nestjs/src/jobs.service.ts`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/api-nestjs/src/jobs.service.ts)
- [`nextjs/package.json`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/nextjs/package.json)
- [`nextjs/src/lib/search.ts`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/nextjs/src/lib/search.ts)
- [`nuxtjs/package.json`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/nuxtjs/package.json)
- [`nuxtjs/server/api/jobs.get.ts`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/nuxtjs/server/api/jobs.get.ts)
- [`expo-react-native/package.json`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/expo-react-native/package.json)
- [`expo-react-native/App.tsx`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/expo-react-native/App.tsx)
- [`.github/workflows/ci-expo-react-native.yml`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/.github/workflows/ci-expo-react-native.yml)
- [`nuxtjs/Dockerfile`](https://github.com/aqutw/auto-job-site/blob/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e/nuxtjs/Dockerfile)

變更依據：

- [`455678b`](https://github.com/aqutw/auto-job-site/commit/455678bf774f457a01e1ed57c49f345343278313)：feat: complete PoC with Golang and NextJS
- [`e0393a1`](https://github.com/aqutw/auto-job-site/commit/e0393a1de2129b7c605094fb0c9f2ab5ddca5685)：feat: API endpoints made by NestJS (NodeJS)
- [`615f48c`](https://github.com/aqutw/auto-job-site/commit/615f48c32d68695d73f118663633592390fdb18f)：feat: make NuxtJS website with VueJS
- [`cc71480`](https://github.com/aqutw/auto-job-site/commit/cc7148079b4340eec0c347a6721ce75e03678278)：feat: add iOS APP
- [`425500d`](https://github.com/aqutw/auto-job-site/commit/425500d0e14bfcb314bebe5c959b0a44d53bbfd5)：fix: API host issue in Android Simulator
- [`f09621f`](https://github.com/aqutw/auto-job-site/commit/f09621faacbf5e8ea862ece3eb8c93a8cd1de13e)：feat: completly tested http://localhost:3001/ using docker container

範圍說明：API 的搜尋條件最多五個關鍵字並以 AND 組合。此 repo 消費既有職缺資料與範例 SQLite，未將外部爬蟲算成 repo 內功能。Mobile 具有 iOS 與 Android 設定，Android commit 修正 LAN HTTP 存取。

## go-api

Go／Gin GitOps 練習，提供 health、version、示範 users 與 Prometheus metrics；附 GHCR 映像建置流程，以及 Kubernetes、Kustomize、Argo CD 與 Image Updater 設定範例。

主要技術：`Go` `Gin` `Prometheus` `Docker` `GHCR` `Kubernetes` `Kustomize` `Argo CD` `GitHub Actions`。

檢查版本：[`2c16c79`](https://github.com/aqutw/go-api/commit/2c16c795493264bccd6d17ac1a97b0f5297681d3)。

檔案依據：

- [`go.mod`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/go.mod)
- [`main.go`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/main.go)
- [`Dockerfile`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/Dockerfile)
- [`.github/workflows/ci.yml`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/.github/workflows/ci.yml)
- [`k8s/deployment.yaml`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/k8s/deployment.yaml)
- [`k8s/kustomization.yaml`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/k8s/kustomization.yaml)
- [`k8s/application.yaml`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/k8s/application.yaml)
- [`k8s/image-updater.yaml`](https://github.com/aqutw/go-api/blob/2c16c795493264bccd6d17ac1a97b0f5297681d3/k8s/image-updater.yaml)

變更依據：

- [`f7cd708`](https://github.com/aqutw/go-api/commit/f7cd708d62a0b8eb63adbcecfce47e44c6620164)：Add GitHub Actions CI
- [`4dad506`](https://github.com/aqutw/go-api/commit/4dad5067d5a669075cc8672aab2e89f77f3ea02a)：add go-api-app.yaml and k8s/kustomization.yaml
- [`08e5ad9`](https://github.com/aqutw/go-api/commit/08e5ad9f89daaa07b98bbf65b53dc32d84c9817d)：add k8s/image-updater.yaml and k8s/application.yaml
- [`2c16c79`](https://github.com/aqutw/go-api/commit/2c16c795493264bccd6d17ac1a97b0f5297681d3)：feat: add version endpoint

範圍說明：main.go 實際提供 /health、/version、/users、/metrics。go.mod 雖列出 MongoDB driver，程式未使用，因此未標記 MongoDB。CI 與 Argo CD 指向 main，但預設分支是 master，映像名稱仍含 YOUR_GITHUB_USERNAME；因此僅描述為設定範例，不宣稱自動部署已運作。
