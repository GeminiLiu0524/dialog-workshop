# Dialog 工坊 — Minecraft 對話框生成器

網頁版：見右上角 About 的連結（繁體中文／简体中文／English）

給地圖作者用的 Minecraft **對話框（dialog）** 生成器，支援 1.21.6 以後的版本（含 26.x）。不用安裝、不用寫 JSON，打開網頁就能從零做出多層選單、商店、設定頁這類互動式對話框，一鍵匯出資料包。

> 目前是 **v0.9 測試版**，歡迎回報問題和建議（見下方「回報」）。

## 可以做什麼

- **即時預覽**：右邊是模擬遊戲的畫面，按鈕真的可以按，會開啟其他對話框，送出的指令也會列出來。
- **五種對話框、四種輸入欄位**：多按鈕選單、通知、確認、對話框清單、伺服器連結；文字輸入、勾選框、選項切換、數值滑桿。
- **文字樣式**：16 色與自訂顏色、粗體、斜體、底線、刪除線、亂碼，翻譯鍵、滑鼠提示、點擊動作。
- **免 OP 的指令按鈕**：按鈕直接執行 give、tp 這類指令時，玩家會先看到確認畫面，沒權限的玩家根本執行不了。「執行指令（自動產生資料包）」會改用 `/trigger`，由匯出的資料包代為執行，玩家不需要 OP，也不會看到確認畫面。
- **流程圖**：用心智圖的方式看整個選單怎麼串接。
- **讀別人的資料包**：直接選 .zip、資料包資料夾，甚至整個世界資料夾，就能打開裡面所有的對話框。
- **專案**：自動存在瀏覽器裡，也可以下載成 `.dlgproj.json` 備份或分享。
- **檢查**：會標出遊戲不接受的設定（例如選單沒有按鈕、用到不存在的鍵名）。

## 怎麼用

1. 打開網頁，按「📁 專案」選範本或空白專案。
2. 左邊「＋ 新增」加對話框，中間編輯，右邊預覽。
3. 「📦 匯出資料包」下載 zip，放進存檔的 `datapacks` 資料夾。
4. **離開世界再重新進入**（新的對話框只在進入世界時登錄，`/reload` 不夠）。
5. 遊戲裡打 `/dialog show @s <命名空間>:<ID>`。

## 回報

- 網頁右上角的「💬 回報問題」會打開回報表單，版本、瀏覽器、語言會自動填好（需要 GitHub 帳號）。
- 回報時請附上：做了哪些步驟、預期看到什麼、實際看到什麼，有截圖最好。和專案有關的問題，可以把專案檔（`.dlgproj.json`）壓成 zip 一起附上。

## 隱私

所有資料都留在你的瀏覽器裡，不會上傳到任何伺服器。唯一的對外連線是預覽時從 mcasset.cloud 載入原版物品圖示，可以在「⚙ 專案設定」關掉。

## 製作

小冰鳥Icebird（《元素試煉 Elemental Trial》作者）

---

# Dialog Workshop — Minecraft dialog maker (English)

A **Minecraft dialog** maker for map makers, for 1.21.6 and later (including 26.x). No install and no JSON: build multi-level menus, shops and settings screens from scratch in your browser, preview them live, and export a datapack in one click. UI in English, 繁體中文 and 简体中文.

- Live, clickable preview; flow map; all 5 dialog types and 4 input types.
- "Run commands (auto datapack)" buttons use `/trigger`, so players need no OP and never see the confirmation screen.
- Open any datapack `.zip`, datapack folder or whole world folder to read its dialogs.
- Projects are saved in your browser and can be downloaded as `.dlgproj.json`.
- After installing the exported datapack, **leave the world and join again** — `/reload` doesn't register new dialogs.

This is a **v0.9 beta**. Use "💬 Feedback" (top right) to report bugs or suggest ideas — your version, browser and language are filled in for you. Everything stays in your browser; the only outside request is loading vanilla item icons from mcasset.cloud for the preview (can be turned off).
