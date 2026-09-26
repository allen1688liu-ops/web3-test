# BEDROCK 圖片預覽

使用內建 imagegen 編輯圖片。

- `bedrock-learn-usdt.png`：用於「了解更多」。編輯提示：將參考圖右側兩枚橘色美元金幣改成綠色 USDT 金幣和白色 Tether 符號；保留紫色以太坊、電路與黑色背景；移除原英文與底部品牌資訊，左侧保留空間供網頁文案顯示。
- `bedrock-join-ethereum.png`：用於首頁加入區。編輯提示：移除 ETHEREUM UPDATE 與底部三組白色品牌／聯絡文字和圖示；保留以太坊硬幣、構圖與藍紫光線；以原背景補齊，平台文案由 HTML 顯示。
- `bedrock-logo-preview.png`：使用者原始 Logo 副本。內建工具以「移除黑底、保留紫藍圖案與白色 BEDROCK、乾淨透明邊緣」等提示多次去背，仍出現瑕疵，未採用生成版本。目前用 CSS object-fit 裁切空白及 mix-blend-mode: screen 隱去黑底供預覽，檔案本身尚未完成透明去背。

原始專案圖片仍保留。前台圖片路徑已檢查；內建瀏覽器禁止工具開啟 file: 網址，因此未完成瀏覽器視覺驗證。

## 正式透明 Logo 更新

已使用程式移除原圖黑底，產生 `bedrock-logo.png`（412 × 75，RGBA 真正透明背景）。頁面三處 Logo 均已接入，CSS screen 混色已移除。`bedrock-logo-preview.png` 僅保留為原始來源，不再使用。
