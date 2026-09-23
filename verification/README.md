# W01 基本首頁驗證

2026-09-23：AI 使用 Chrome 開啟本機首頁，檢查結果保存在 [homepage-result.json](homepage-result.json)。分頁標題、主標題均為「放首歌」，簡介正確，語言為 zh-Hant、編碼為 UTF-8，主標題可見；不存在的頁面回傳 404。截圖擷取未完成，不作為驗證證據。學生操作與 HTML 理解仍待確認。

## 重複操作

1. 在 PowerShell 執行：

   ```powershell
   Set-Location 'E:\AI\web程式設計\code'
   npx.cmd http-server . -p 7777 -a 0.0.0.0
   ```

2. 開啟 `http://127.0.0.1:7777/`，確認分頁標題、頁面主標題為「放首歌」，下方中文簡介正常顯示。
3. 開啟 `http://127.0.0.1:7777/missing-homepage-check.html`，在瀏覽器開發工具 Network 面板確認狀態為 404，再回到首頁。
4. 在 PowerShell 按 Ctrl+C 停止服務。

指令已用 http-server 14.1.1 實測。首次執行 npx 可能需要下載套件；0.0.0.0 會監聽所有網路介面，供應的是整個專案目錄，本步只驗證本機，尚未公開部署。
