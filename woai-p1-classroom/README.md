# 小一《我愛學語文》課文互動遊戲 · GitHub Pages

建議倉庫名稱：`woai-p1-classroom`

## ⚠️ 上傳方法（必讀）

**一定要這樣上傳，否則會出現 Jekyll `dir_chdir …/docs` 錯誤：**

1. 在 GitHub 建立一個**空的 Public** repository（建議名：`woai-p1-classroom`）。
2. 打開本資料夾 `woai-p1-classroom/`，上傳時**只選裡面的兩個項目**：
   - `README.md`
   - `docs/`（資料夾）
3. **不要**再包一層「某某網站」或 `woai-p1-classroom` 父資料夾再上傳。  
   Repo **根目錄必須直接見到** `docs/` 與 `README.md`。
4. 前往 **Settings → Pages**
   - Source：Deploy from a branch
   - Branch：`main`
   - Folder：**`/docs`**
5. 儲存後稍等一兩分鐘，網站網址會是：

   https://nhto.github.io/woai-p1-classroom/

## 為何會失敗？

若把成個中文／外層資料夾一併上傳，真正檔案會落在 `某某網站/docs/`，Pages 搵唔到根目錄 `/docs`，就會出現：

```
Error: No such file or directory @ dir_chdir0 - /github/workspace/docs
```

本套件已包含空檔 `docs/.nojekyll`，避免 GitHub Pages 的 Jekyll 處理破壞靜態 HTML。

## 內容

- `docs/index.html`：入口頁（卡片連本地遊戲；二維碼以 QRCode.js 動態產生本站絕對網址）
- `docs/我愛學語文課文互動遊戲/`：9 個課文情景互動遊戲
- `docs/.nojekyll`：略過 Jekyll
