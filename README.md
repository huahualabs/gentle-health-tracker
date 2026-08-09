# 好好照顧自己｜手機 PWA 版

這一版的目標是：Mac 關機也能使用、人在外面也能開、可加入 iPhone 主畫面、資料仍只保存在自己的 iPhone 瀏覽器。

## 隱私設計
- GitHub Pages 上只放「空白程式模板」，不把私人健康清單寫進公開程式碼。
- 第一次在 iPhone 開啟後，可匯入自己從舊版匯出的 JSON 備份。
- JSON 備份不要上傳到 GitHub repository。
- 日常紀錄使用 localStorage，關閉分頁不會自動消失。

## iPhone 使用方式
1. 用 Safari 打開 GitHub Pages 網址。
2. 第一次使用，匯入自己的私人 JSON 備份。
3. Safari 分享 → 加入主畫面。
4. 之後從主畫面的「照顧自己」圖示開啟。

## 離線
已包含 Service Worker。成功開啟網站至少一次後，主要頁面可在沒有網路時載入。

## GitHub Pages
這是純靜態網站，不需要 Node、Firebase 或伺服器。
把本資料夾中的公開網站檔案放在 repository 根目錄，Pages 使用該 branch 的 /(root) 發布即可。

## 請勿上傳
- health-tracker-backup-*.json
- 任何含私人健康資料的 JSON
