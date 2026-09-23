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

## W02 單首靜態歌曲（2026-09-23）

- 原版參考：`C:/Users/user/Documents/Codex/2026-07-31/new-chat/app/test/motion-player.tsx` 的歌曲列表（歌名在前、歌手在後、ol/li 結構），及 `db/songs.ts` 的初始範例「逍遙仙／三無Marblue」。只讀取原檔，未複製播放器與動態狀態；尚未加入 CSS。
- Chrome 實測結果見 [song-list-result.json](song-list-result.json)：主標題與 h2/h3 層級、區域名稱、一首歌曲及歌手可見、不存在頁面 404 均通過。這是 DOM 與可見尺寸檢查，未取得截圖，不代表完整視覺驗收。
- 重複步驟：依上方指令啟動服務，開啟 `http://127.0.0.1:7777/?check=w02`；應依序看見「放首歌」、原簡介、「歌曲列表」、編號 1、「逍遙仙」及「歌手：三無Marblue」。重新整理後內容應保持一致。
- 開啟 `/missing-song-check.html`，在 Network 確認 404；回到首頁仍應正常顯示。完成後在啟動服務的 PowerShell 按 Ctrl+C。

## W02 第二首歌曲

AI 依學生要求在同一 ol 加入「伴我／張靚穎」。Chrome 結果見 [two-songs-result.json](two-songs-result.json)：列表數量 1、兩個 LI、decimal 編號樣式、兩首歌名與歌手可見。重複檢查：沿用上方啟動指令，開啟 `http://127.0.0.1:7777/?check=w02-two`，應依序看見 1. 逍遙仙／三無Marblue、2. 伴我／張靚穎。此輪只擴充靜態項目，未重跑先前已通過且未受影響的 404 檢查。
