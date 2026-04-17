智能發票管家 PWA — 安裝說明
================================

方法一：解壓縮後用任何 HTTP 伺服器提供服務（推薦）
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
1. 解壓縮 invoice-app.zip
2. 上傳整個資料夾到任何網頁空間（例如 GitHub Pages、Netlify、Vercel 等免費服務）
3. 手機用瀏覽器開啟網址
4. Android（Chrome）：點選右上角選單 → 「加入主畫面」
   iPhone（Safari）：點選分享按鈕 → 「加入主畫面」

方法二：直接用本機伺服器（電腦測試）
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
python3 -m http.server 8080
（在 invoice-app 資料夾中執行，然後開啟 http://localhost:8080）

注意事項
━━━━━━━
• PWA 必須在 HTTPS 或 localhost 環境下才能安裝
• 單純用 file:// 開啟 HTML 語音辨識無法使用
• 資料儲存在瀏覽器 localStorage，清除瀏覽器資料會同時清除 App 資料
• 建議使用 GitHub Pages（免費、HTTPS、永久網址）

GitHub Pages 快速部署
━━━━━━━━━━━━━━━━━━━━
1. 申請 GitHub 帳號
2. 建立新 Repository（設為 Public）
3. 上傳 invoice-app 資料夾的所有檔案
4. Settings → Pages → Source 選 main branch
5. 幾分鐘後網址：https://你的名字.github.io/repository名稱/
