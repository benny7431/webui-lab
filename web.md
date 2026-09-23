# 網頁學習紀錄

## 2026-09-21：W01 環境與 Git 起步

### 本次目標與成果

- 目標：啟用「放首歌」的本機 Git 版本紀錄，檢查忽略規則，設定只適用於本專案的提交署名。
- AI 已檢查：Node.js、npm、Git 能執行；儲存庫分支為 `main`；11 項忽略規則檢查通過；署名設定來自本專案的 `.git/config`。
- 學生已操作：在 PowerShell 切換至專案資料夾，執行 `git status` 並貼回結果；也執行兩個 `git config --local --get` 指令，確認姓名與 email。
- 目前尚無任何 commit，尚未執行 `git add`、`git commit` 或推送 GitHub。

### 概念與理解確認

- `--local`：設定目前這個 Git 專案，內容存在專案自己的 `.git/config`。
- `--global`：設定目前使用者的共用預設值；專案有自己的設定時，會優先使用專案設定。
- 理解已確認的範圍：學生在「只替另一個專案設定不同署名」的情境中，回答應使用 `--local`。
- 學生能判斷目前沒有舊版本可還原，原先理由是「之前沒有追蹤」。AI 補充：此處的直接證據是 `No commits yet`。
- `git add` 與 `git commit` 的差別已講解，尚待學生實際操作與確認理解。

### 待完成

- 基本首頁、README、第一筆提交與 GitHub 上傳仍待完成。
- 學生尚未提供本次個人心得；本紀錄僅整理實際操作與回答，不代表整週 W01 已完成。

## 2026-09-23：W01 暫存第一個檔案

- 學生已操作：在專案目錄執行 `git add .gitignore` 與 `git status`，貼回 `.gitignore` 位於 `Changes to be committed`、其他檔案未追蹤及 `No commits yet` 的輸出。
- AI 已檢查：實際暫存區只有 `.gitignore`，內容為既有忽略規則；`core.autocrlf=true`，LF／CRLF 警告未造成暫存失敗，沒有更改 Git 設定。
- 已說明：暫存是選入下一次提交的內容；尚未建立 commit 或上傳 GitHub。LF 與 CRLF 是不同換行格式。
- 理解待確認：請學生判斷照目前狀態建立一次 commit 會包含哪些檔案，並說明理由；尚未收到回答，不記為已理解。

## 2026-09-23：W01 README 與基本首頁

- 學生已操作：修改 README 並回報完成；回答「沒ｈｔｍｌ阿」，確認 README 不會自動產生 HTML 首頁。
- 學生同意基本首頁方案，AI 建立 index.html，說明 title、h1、p 的用途。
- AI 已檢查：Chrome 本機首頁標題、簡介、UTF-8、zh-Hant 與主標題可見性；不存在頁面回傳 404。證據與重複步驟見 verification/README.md。
- 理解已確認：學生能判斷只改 title 會改變分頁名稱、h1 不隨之改動；回答中的「釋放首歌」已更正為原文「放首歌」。學生隨後明確回報已親自在瀏覽器看到首頁並授權提交；其餘 HTML 理解不擴大認定，沒有代寫心得。
