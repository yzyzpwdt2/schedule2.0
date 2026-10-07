# 北市勤務排程 2.0

勤務排程的獨立介面改版。原始 `schedule` repository 不受影響。

## 畫面

- `index.html`：勤務總覽。提供全部／今天／7 天內／後續篩選、工程師篩選、全文搜尋、依日期分組、備註展開、同步狀態、快取與每分鐘自動同步。
- `admin.html`：新增勤務與近期排程。提供欄位驗證、工程師選取、排程搜尋及手動重新整理。

## 資料來源

前端沿用 `config.js` 的 `SCHEDULE_API_URL`，透過既有 Google Apps Script API 讀取與新增勤務。Apps Script 程式碼與試算表欄位格式保持相容。

部署時將前端檔案發布到 GitHub Pages，並確認 `config.js` 指向正確的 Apps Script 網頁應用程式網址。
