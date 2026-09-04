# Personal Memo 專注守門員隱私權政策

生效日期：2026 年 9 月 4 日

Personal Memo 專注守門員（以下稱「本擴充功能」）是 Personal Memo Windows 桌面程式的搭配工具。本政策說明本擴充功能存取哪些資料、如何使用資料，以及使用者可以如何控制功能。

## 存取與處理的資料

只有在下列條件同時成立時，本擴充功能才會讀取目前作用中分頁的網址：

1. 同一台電腦上的 Personal Memo 正在執行。
2. 使用者已開始一輪含有允許網域規則的專注計時。

本擴充功能只從目前網址取出網域名稱（hostname，例如 `docs.google.com`）。本擴充功能不讀取或收集頁面內容、頁面標題、查詢參數、路徑、表單內容、密碼、下載內容，或瀏覽紀錄清單。

## 資料傳輸、保存與分享

網域名稱只會送到同一台裝置上的 Personal Memo 本機服務（`http://127.0.0.1:38473`），用來判斷目前網站是否在本輪專注模式的允許範圍內。

- 不會把資料傳送到 Personal Memo 的雲端、開發者伺服器或任何第三方。
- 不會保存網域名稱或建立瀏覽紀錄。
- 不會出售、出租或用於廣告、信用評分、個人化行銷或使用者追蹤。
- 不會把資料用於本功能單一目的以外的用途。

## 權限用途

- `tabs`：在專注模式進行時取得目前作用中分頁的網址，並只取出網域名稱。瀏覽器可能因此顯示與「瀏覽活動」或「瀏覽紀錄」相關的標準權限文字；本擴充功能不會呼叫瀏覽器的 History API，也不會讀取瀏覽紀錄清單。
- `http://127.0.0.1:38473/*`：與同一台電腦上的 Personal Memo 桌面程式通訊。此權限不允許本擴充功能連線到其他網站或雲端服務。

## 效能設計

本擴充功能使用瀏覽器的分頁與視窗事件觸發檢查，不使用持續輪詢計時器。沒有相容的專注計時時，本擴充功能不會讀取作用中分頁。

## 使用者控制

使用者可以隨時在 Personal Memo 結束專注計時、移除允許網域規則、停用本擴充功能或解除安裝本擴充功能。解除安裝後，本擴充功能不再存取任何瀏覽器資料。

## 政策更新與聯絡方式

如本政策有重大變更，我們會在公開發布頁與擴充功能商店頁面更新說明及生效日期。如有隱私、錯誤或功能建議，請透過 [Personal Memo 問題與優化回報](https://github.com/lk242/personal-memo-releases/issues) 聯絡我們。

---

# Personal Memo Focus Guard Privacy Policy

Effective date: September 4, 2026

Personal Memo Focus Guard (the “Extension”) is a companion to the Personal Memo Windows desktop app. This policy explains what data the Extension accesses, how it is used, and the controls available to users.

## Data accessed and processed

The Extension accesses the active tab URL only when both conditions are true:

1. Personal Memo is running on the same computer.
2. The user has started a focus session that contains an allowed-domain rule.

Only the hostname (for example, `docs.google.com`) is derived from the active URL. The Extension does not read or collect page content, page titles, query parameters, URL paths, form contents, passwords, downloads, or browsing-history lists.

## Data transmission, retention, and sharing

The hostname is sent only to Personal Memo's local service on the same device at `http://127.0.0.1:38473`. It is used to determine whether the current website is within the focus session's allowed domains.

- Data is not sent to Personal Memo cloud services, developer servers, or third parties.
- Hostnames are not retained and no browsing history is created.
- Data is not sold, rented, or used for advertising, credit scoring, personalized marketing, or user tracking.
- Data is not used for any purpose outside the Extension's single purpose.

## Permission use

- `tabs`: obtains the active tab URL during a focus session and derives only its hostname. The browser may display standard permission language related to browsing activity or browsing history. The Extension does not use the browser History API and does not access browsing-history lists.
- `http://127.0.0.1:38473/*`: communicates with the Personal Memo desktop app on the same computer. This permission does not allow the Extension to connect to other websites or cloud services.

## Performance design

Checks are triggered by browser tab and window events. The Extension does not use a continuous polling timer. When no compatible focus session is running, the Extension does not access the active tab.

## User controls

Users can end the focus session, remove allowed-domain rules in Personal Memo, disable the Extension, or uninstall it at any time. After uninstalling, the Extension no longer accesses browser data.

## Updates and contact

If this policy changes materially, the effective date and relevant notices will be updated on the public release page and extension store listing. For privacy questions, bug reports, or improvement suggestions, contact us through [Personal Memo Issues and Improvements](https://github.com/lk242/personal-memo-releases/issues).
