# 放首歌：目前進度

最後更新：2026-09-23 15:53:09 +08:00（Asia/Taipei）

## 目前停留點

最新回覆：針對窄視窗確認及整理提交，學生回覆「可以～」。依上下文作為窄視窗顯示正常及本機提交同意；未取得具體視窗尺寸，不宣稱實體手機測試。AI 已核對 CSS、首頁連結及既有 958px／375px 驗證結果，本輪準備提交「W02: 加入 Noir 基礎配色與版面間距」，不上傳新提交。HTML／CSS 分工情境已答對，渲染用詞已補充。

本輪接續：學生已同意基本首頁方案，AI 新增 index.html 並以 Chrome 實測本機首頁的標題、簡介、中文編碼及主標題可見性；不存在頁面回傳 404。結果與重複操作見 verification/README.md、homepage-result.json；截圖擷取逾時，沒有截圖證據。title 與 h1 的修改影響已確認；學生已確認親自開啟首頁；其餘 HTML 理解不擴大認定。首次提交已授權。學生提醒網頁應盡量參考原專案，已核對 AGENTS 與 ROADMAP B／C：後續結構及 Noir 外觀需先讀取原版對應檔案再調整；本輪基本首頁尚未取用原版畫面。

目前進入 W02 單首靜態歌曲；以下保留 W01 已確認成果及待確認概念。Git 初始化、忽略規則檢查及本專案提交署名設定已完成；學生已貼回署名查詢結果，並在情境題中正確選擇 `--local`。學生已親自執行 `git add .gitignore` 與 `git status`，暫存操作成功；暫存概念理解仍待回答；現已完成首次 commit。學生已完成 `README.md` 標題與簡介修改並回報，AI 已核對內容；README 不會自動產生 HTML 首頁的基本理解已確認；整週 W01 尚未完成。

學生指出先前代理把 Git 理解題排在 README 之前，並質疑 `npm run dev` 是否屬於最新教材。本輪重新讀取 [WEB03 整合版](https://moodle.ncnu.edu.tw/pluginfile.php/170589/mod_resource/content/0/web03.md)，確認同份文件含 W01、W02、W03；W01 第 1.7 節 README 範例只有標題、簡介與學號，首頁段落改用 7777 埠的 `http-server`。較早的 [獨立 WEB01](https://moodle.ncnu.edu.tw/pluginfile.php/162581/mod_resource/content/0/web01.md)才在 README 範例列 `npm install`／`npm run dev`，不可混為最新版本。現行順序是 `.gitignore` → README → `index.html` → 第一次 commit → GitHub；教材對照保留於下方。

本輪依使用者要求，已更新 `AGENTS.md`、`ROADMAP.md`、`ai.md` 及本進度文件的教材版本、教學接續與實際檔案狀態；沒有更動 `.github/copilot-instructions.md`、學生正在編輯的 `.gitignore` 或現有 README。WEB03 的 W03 以已有網站 demo 為前提，學生可依修課情形使用靜態伺服器或 FastAPI，IIS／HTTPS 由老師設定；這些部署操作尚未在本專案進行。

## 已完成與目前狀態

- 專案名稱已確定為「放首歌」，是獨立從零建立的歌曲網站。
- 現有檔案包含 `.gitignore`、`README.md`、`AGENTS.md`、`.github/copilot-instructions.md`、`PROGRESS.md`、`ROADMAP.md`、`web.md`、`ai.md`，另有 index.html 與 verification/；均已納入首次提交。
- 本輪在 Moodle 登入頁核對 WEB03 的 W01／W02／W03 內容與舊 WEB01 的差異，並核對實際檔案及 Git 狀態；文件修正僅涉及 `AGENTS.md`、`ROADMAP.md`、`PROGRESS.md`、`ai.md`。代理未代學生暫存、提交、推送或新增應用程式。
- 最新 Git 狀態：main 與 origin/main 同步於 a24bdaa；CSS、首頁載入連結及本輪學習／驗證紀錄尚未提交。
- Git 名稱與 email 已設定在本專案，學生也已查詢並貼回正確結果。具體值由 `git config --local --get user.name` 與 `git config --local --get user.email` 查詢，不需再次索取或重做設定。
- 主對話已有檢查證據：Node.js、npm、Git 能執行，11 項忽略規則檢查通過。本輪沒有重跑這些檢查。
- 已有基本 `index.html` 及實測可用的 http-server 啟動方式；已有兩首靜態歌曲展示；尚無 `package.json`、播放功能或公開部署。

## 已確認決定與待取得資訊

- 期末以完整 Noir 專題為目標，包含音訊特效與 AI 整理；依老師每次提供的 MD 從功能地圖取用，沒有固定每週功能表。
- 平時深入學習課程核心；進階功能可由 AI 協助整合，學生要能說明用途、流程、來源、調整與驗證，不要求逐行推導所有進階演算法。
- 最後一週可集中補齊與整合，期末前先核對剩餘工作量、音源、AI 服務與部署依賴。完整目標不自行刪減，也不預設延後到課後。
- 原專案僅唯讀參考；固定參考版本及技術建議見 `ROADMAP.md`。正式課綱、期末期限與評分細節仍待教材確認，音源、部署限制及 AI 預算到相關階段核對。

## 2026-09-23 教材對照與來源

最新取得的 WEB03 整合版已從登入中的 Moodle 原文核對，包含 W01、W02、W03；老師原文未修改。較早獨立版只供辨認版本差異。下方其他來源與上傳時間沿用同日先前的 Moodle 核對紀錄。

| 教材／段落 | 已核對內容 | 對照本專案 |
|---|---|---|
| [WEB03 W01／W02／W03 整合版](https://moodle.ncnu.edu.tw/pluginfile.php/170589/mod_resource/content/0/web03.md)，[資源頁](https://moodle.ncnu.edu.tw/mod/resource/view.php?id=91739&forceview=1)；上傳 2026-09-20 16:51 | W01 建檔順序為 `.gitignore`、README、`index.html`、初次 commit；這版 README 範例無 `npm run dev`，首頁可用 `http-server` 7777。W02 是 HTML／CSS、語意標籤、Project Milestone 與學習紀錄；W03 是本機到公開部署。 | 以此版處理目前課程進度。較舊獨立 WEB01 的 `npm run dev` 與 3000 埠範例只作版本對照，不成為本專案指令。 |
| [WEB02 獨立版](https://moodle.ncnu.edu.tw/pluginfile.php/167403/mod_resource/content/0/web02.md)，[資源頁](https://moodle.ncnu.edu.tw/mod/resource/view.php?id=89121&forceview=1)；上傳 2026-09-13 23:58 | 依專案需求設計簡單 HTML/CSS，CSS 放 `css/`；理解語意化標籤；整理 Project Milestone（問題、使用者、功能、資料、API、風險、MVP），留下 W02 學習紀錄。ChatGPT 風格是教材示例。 | WEB03 已包含 W02 相同主題；尚無 HTML/CSS 畫面或語意化標籤操作／理解證據。仍須整理明確的問題、使用者與最小可展示版本，不必重做整份路線圖。 |
| [WEB03 原文](https://moodle.ncnu.edu.tw/pluginfile.php/170589/mod_resource/content/0/web03.md)，[資源頁](https://moodle.ncnu.edu.tw/mod/resource/view.php?id=91739&forceview=1)；上傳 2026-09-20 16:51；`W03 — 從本機開發到公開部署` Part 3 | 預設已有 demo。只修 Web Programming 者可用 `npx.cmd http-server . -p 7777 -a 0.0.0.0`；FastAPI 是可選路徑。老師收集 IP、設定 IIS 反向代理與 HTTPS，學生測試本機和公開網址。 | 對應 ROADMAP A／B／C 與 I 的早期部署；目前缺首頁及已驗證啟動方式，不應直接安裝整套 Python／IIS。尚未確認學生是否兼修 DBS、實際主機／網路、正式公開網址及老師 IP 登記方式；教材 `https://demo…/` 是示意，不能當成可用網址。 |
| [W03 課程單元](https://moodle.ncnu.edu.tw/course/view.php?id=7757)，2026-09-20 至 09-26 | 另有 HTML 影片、W3Schools 練習及 HTML Quiz；課程要求隨影片暫停、互動並驗證。另份 IIS／Uvicorn 詳細文件明標給 TA 參考、有興趣自學。 | 影片、練習與 Quiz 完成情形沒有本專案證據，保持待確認；不把伺服器管理員的工作列成學生必裝項目。 |
| [Check Point #1 簡報專題計畫](https://moodle.ncnu.edu.tw/mod/assign/view.php?id=80057)，置於 W04（2026-09-27 至 10-03） | 每組一人上傳；兼修兩門課者交於資料庫系統；標題頁列姓名、學號、角色；上傳後保持草稿，不按正式繳交。本次頁面未列明確截止時間。 | 此 Web 作業頁顯示尚無提交；不能據此斷言資料庫課也未交。企畫可取用 ROADMAP，是否組隊／兼修 DBS 及簡報準備情形待確認；W04 單元日期不當成截止日。 |
| [AI 使用規範](https://moodle.ncnu.edu.tw/pluginfile.php/167400/mod_resource/content/0/web_AI_rules.md) 第 4、5、7 節 | 小步實作、瀏覽器驗證、檢視差異再提交；每週至少 3 次實質 commit，訊息用 `W<週次>: ...`，週五或指定期限前 push；更新 `web.md`／`ai.md`。 | 現已有 2 筆 commit，兩筆均已上傳 origin/main；每週紀錄及實質進度持續累積，不能據此宣稱 W02／W03 學習已完成。 |

部署時需驗證學校 IIS 能連到所用主機；只提供私人網路 IP 不代表可達。公開網址含學號子路徑時，須在該網址實測 CSS／圖片／連結；伺服器程序停止後網站會失去服務。這些是後續操作的驗證點，本輪未更動防火牆或網路設定。

## 學生操作與理解

| 項目 | AI 已檢查 | 學生已操作 | 理解證據與待確認事項 |
|---|---|---|---|
| Git 初始化 | 儲存庫與 `main` 已核對 | 學生已切換至專案資料夾並貼出 `git status`，當時顯示 `No commits yet` 與三個未追蹤項目 | 學生回答目前不能還原舊版本，理由是之前沒有追蹤。AI 已補充關鍵是尚無 commit；後續暫存操作見下列紀錄，概念差別仍待學生回述 |
| 本專案 Git 署名 | 名稱、email 與本機專案設定範圍已核對 | 學生已執行兩個 `git config --local --get` 指令並貼回結果 | 已說明專案 `.git/config` 與共用預設值的差別；學生在「只改另一個專案署名」的情境中回答 `--local`，適用情境的選擇已確認 |
| Git 暫存 | 已核對只有 `.gitignore` 在暫存區，內容為既有忽略規則；換行警告未造成暫存失敗 | 學生執行 `git add .gitignore`、`git status` 並貼回輸出 | 操作已確認；待回答目前直接提交會包含哪些檔案及理由，不把操作成功當成理解已確認 |
| README | 已核對標題「放首歌」、以目標描述的歌曲網站簡介及既有學號欄；沒有本機執行指令 | 學生回報修改完成，與實際檔案一致 | 學生回答「沒ｈｔｍｌ阿」，已確認理解目前尚缺 HTML 首頁；不據此推定已理解 HTML 標籤 |
| 進度與學習紀錄 | 本輪核對 WEB03 整合版並更新專案指引、路線圖、進度與 AI 協作紀錄 | 學生已回報暫存結果、指出應先接 README，並提供目前最新教材；尚未提供暫存概念回答或心得 | 依 WEB03 逐步核對現有 README，再做首頁；文件更新不等於學生已操作或理解 W02／W03 |

## 下一個接續點

1. 不重做 Git 初始化、署名設定或已成功的 `.gitignore` 暫存操作；先前提出的暫存理解題待答，但不擋住 README 或首頁。
2. README 操作、首頁瀏覽器操作及 title／h1 的差別已確認，不重考；學生已授權首次提交。
3. 首次提交與 GitHub 上傳已完成；請學生親自查看 webui-lab 的 README、index.html 與提交紀錄，學生已正確指出 push 負責上傳提交，這項不重考。不重做初始化、遠端設定或首次推送。
4. 兩首歌曲已提交並推送。CSS 基礎配色與間距已由 AI 完成並檢查；學生已回報 CSS 畫面出現；HTML 內容與 CSS 外觀分工的情境已答對，渲染一詞已補充說明；學生已回覆窄視窗可用並同意提交；本輪提交後可再安排下一個課程小目標。
