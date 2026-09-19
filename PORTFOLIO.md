# GitHub Copilot 實戰工作坊待辦清單 Web App

這是一個在 GitHub Copilot 實戰工作坊中完成的待辦清單 Web App。專案以簡潔的介面提供日常待辦事項管理功能，並透過主題切換與篩選功能，示範如何從需求逐步完成可操作的前端作品。

## 線上展示

[GitHub Pages](https://<你的帳號>.github.io/<你的repo名稱>/)

> 請將上方網址中的 `<你的帳號>` 與 `<你的repo名稱>` 替換成實際的 GitHub 帳號與 repository 名稱。

## 功能

- 新增待辦事項，並限制內容長度與避免提交空白內容。
- 將待辦事項標記為已完成，或取消完成狀態。
- 刪除單筆待辦事項。
- 依照「全部」、「未完成」與「已完成」篩選待辦事項。
- 在清單沒有內容或篩選結果為空時，顯示對應的提示訊息。
- 顯示目前未完成的待辦事項數量。
- 依照作業系統的 `prefers-color-scheme` 偏好初始化淺色或深色模式。
- 透過按鈕手動切換淺色與深色模式。
- 保存待辦事項與主題偏好，重新載入頁面後仍可保留。
- 提供鍵盤焦點樣式、ARIA 標籤與螢幕閱讀器輔助文字。
- 支援小螢幕版面配置。

## 技術

- 使用純 HTML、CSS 與原生 JavaScript。
- 不使用任何前端框架或第三方套件。
- 不依賴外部 CDN，可離線運作。
- 使用 CSS 自訂屬性集中管理顏色與主題配色。
- 使用瀏覽器 `localStorage` 保存待辦資料與使用者的主題偏好。
- 使用原生 DOM API 產生與更新待辦清單內容。

## 開發方式

這個專案是在 GitHub Copilot 實戰工作坊中，透過以下方式逐步完成：

- **GitHub Copilot Agent Mode**：以自然語言描述需求，讓 Copilot 協助建立待辦清單介面、互動功能與響應式樣式，並依照測試結果持續調整。
- **MCP**：整合 Microsoft Learn 與 GitHub MCP，查詢官方文件、檢視 repository 的 Issue，並以專案內容作為後續修改的依據。
- **`.github/prompts` agentic workflow**：建立可重複使用的 prompt，依序讀取 Issue、提出修改計畫、等待確認、建立分支、修改與驗證、提交推送，最後建立 Pull Request。
- **Git 與 GitHub 工作流程**：以分支、commit、push 與 Pull Request 管理修改，讓每項功能變更都能被追蹤與審查。

## 我學到什麼

- 如何使用 Agent Mode 將一段需求拆解成可執行的前端工作。
- 如何用 CSS 變數與 `prefers-color-scheme` 實作可切換且較容易維護的主題配色。
- 如何使用 MCP 查詢 Microsoft 官方文件與 GitHub Issue，讓 AI 的建議建立在實際資料上。
- 如何設計可重複執行的 prompt，讓 Issue 修復流程包含確認、驗證與 Pull Request。
- 如何在不使用框架或套件的情況下，使用原生 DOM API 與 `localStorage` 完成互動式 Web App。
