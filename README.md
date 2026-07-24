# N5 單字卡（變體版）

一份單檔 HTML 製作的 JLPT N5 單字卡（flashcard）應用，採翻牌式 UI，並支援 Web Speech API 語音朗讀發音。

## 使用方式

直接用瀏覽器開啟 `index.html` 即可使用，無需安裝或建置。

若瀏覽器對 `file://` 開啟的頁面有語音（Web Speech API）限制，可改用簡易伺服器開啟：

```bash
python3 -m http.server
```

再以瀏覽器造訪 `http://localhost:8000`。

## 內容結構

所有單字資料以 `DECK` 物件的形式內嵌於 `index.html` 的 `<script>` 區塊中，依詞性分類（例如 `v1`／`v2`／`v3`／`adj`）。

> 本專案與 `jn5-main` 為同一單字卡概念的不同分支版本，兩者程式碼各自獨立，未共用。
