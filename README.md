### 注意事項
- 用 GitHub Pages 網址，不要用 raw.githubusercontent.com。Pages 的 CORS 允許跨網域，WP 可以直接讀取，速度也比較穩。
- 更新延遲：自動排程最多 15 分鐘，加上 Pages 約 10 分鐘的 CDN 快取，所以急著更新時按選單的手動發佈。
- 日期與時間欄位：getValues() 遇到 Sheet 的日期或時間格式會變成 ISO 字串（時間常變成 1899 年的日期）。你這份課程資料的 time 目前應該是文字，沒問題，但新專案若有日期欄位，需要改用 getDisplayValues()。
- 備援：如果想在 GitHub 讀取失敗時退回 GAS，可以在前端 fetch 失敗時再試原本的 GAS 網址。你要的話我再幫你加。
