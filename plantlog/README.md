# 植物照護

照顧完按一下，記錄澆水、換水、施肥、整理的時間。iPhone 加到主畫面使用。

## 上線（GitHub Pages）
1. GitHub 新增 Public repo，例如 `plantlog`
2. Add file → Upload files，把這個資料夾的檔案全部拖進去 → Commit
3. Settings → Pages → Source 選 Deploy from a branch，Branch 選 `main`、`/ (root)` → Save
4. 約 1 分鐘後網址會是 `https://你的帳號.github.io/plantlog/`

## 加到 iPhone 主畫面
Safari 打開網址 → 分享 → 加入主畫面。之後都從主畫面圖示開啟（和 Safari 裡的資料是分開的）。

## 改版
改完 index.html 重新上傳覆蓋即可，下次打開 App 會抓到新版。
如果改了圖示或想強制更新快取，把 sw.js 第一行的 `plantlog-v1` 改成 `plantlog-v2`。

## 資料
- 存在手機本機（localStorage，key：`plantlog.v1`）
- 設定 → 匯出備份，會產生 JSON 檔，可存到「檔案」或 iCloud
- 之後要接 Google Sheets，只要改 index.html 裡的 `Store` 物件
