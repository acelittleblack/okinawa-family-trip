# 2026 沖繩親子旅行手冊

一頁式互動旅行手冊（PWA），可部署到 GitHub Pages、加到手機主畫面、離線瀏覽。

## 檔案
- `index.html`：互動網頁主檔（行程、美食、玩樂、住宿・航班、天氣、醫療、待辦）
- `manifest.webmanifest` / `sw.js`：PWA 設定與離線快取
- `assets/`：App 圖示
- `.nojekyll`：讓 GitHub Pages 直接輸出

## 部署（GitHub Pages）
1. 建立 public repository 並上傳本資料夾所有檔案。
2. `Settings` → `Pages` → Source 選 `Deploy from a branch`，Branch 選 `main` / `(root)`。
3. 儲存後等待產生網址。

## 更新內容
修改 `index.html` 後，把 `sw.js` 的 `CACHE_VERSION` 版本號 +1，已安裝的離線快取才會更新。
