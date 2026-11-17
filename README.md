# 週日誌 Weekly Planner

一個以 HTML、CSS 與原生 JavaScript 製作的響應式週計畫網站。資料存在目前瀏覽器的 `localStorage`；首次開啟會載入範例資料。網站沒有建置步驟，可直接部署到 Vercel。

## 本機預覽

直接用瀏覽器開啟 `index.html`，或在專案資料夾執行：

```sh
npx serve .
```

Chart.js 從 jsDelivr CDN 載入，因此圖表需要網路連線。

## 上傳 GitHub

在 GitHub 建立空白 repository，然後於此資料夾執行：

```sh
git init
git add index.html styles.css app.js vercel.json README.md
git commit -m "Build weekly planner"
git branch -M main
git remote add origin https://github.com/<your-name>/<your-repo>.git
git push -u origin main
```

## 部署 Vercel

在 Vercel 選擇 **Add New → Project**，匯入剛建立的 GitHub repository。Framework Preset 選 **Other**，Build Command 與 Output Directory 留空，然後部署。之後推送到 `main` 會自動重新部署。

## 備份與資料

使用頁面右上角的匯出功能下載 JSON 備份；換瀏覽器或裝置時匯入備份即可。`localStorage` 資料只存在當前瀏覽器，不會自動同步至 GitHub 或其他裝置。

