# 範例高中網站

「檢索增強生成與客製化聊天機器人實作」課程用的虛構學校網站。

- 內容與「校園資訊助理」的知識庫 `campus.csv` 相同，共 970 則（已排除 30 筆雜湊雜訊）。
- 每則內容的資料網址（`https://fanli-high.github.io/#…`）就是聊天機器人回答時列出的來源，與 `campus.csv` 的 url 欄位一致。
- 單一靜態頁面 `index.html`，不需要伺服器程式或資料庫。
- 已設定 `noindex`，搜尋引擎不會收錄這個虛構學校。

## 換成自己學校

`index.html` 最後的 `<script type="application/json" id="data">` 區塊就是資料，每則格式如下：

```json
{"id":"reg-001","cat":"reg","t":"標題","k":"關鍵字, 以逗號分隔","c":"內容"}
```

修改後重新上傳 `index.html`，GitHub Pages 約一分鐘後就會更新。
