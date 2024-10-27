# LinSpeedWeb 連結預先載入優化腳本
优化网页载入速度

## 描述

這是一個 Tampermonkey 使用者腳本，用於當滑鼠移動到網頁連結時預先載入該連結，並屏蔽所有帶有下載屬性的連結。此腳本有助於提升網頁的加載速度和使用體驗。

## 功能

- **連結預先載入**：當滑鼠移動到連結時，自動預先載入該連結的資源，以加快頁面加載速度。
- **屏蔽下載連結**：自動識別並屏蔽所有帶有 `download` 屬性的連結，防止不必要的下載行為。
- **動態監控**：使用 `MutationObserver` 監控動態添加的連結，確保所有新加入的連結都受到腳本的管理。

## 安裝

1. **安裝 Tampermonkey**

   若尚未安裝 Tampermonkey，請前往 [Tampermonkey 官方網站](https://www.tampermonkey.net/) 安裝適用於您的瀏覽器的版本。

2. **安裝腳本**

   - **方法一**：點擊 [這裡](https://github.com/您的GitHub帳號/連結預先載入優化腳本/raw/main/prefetch-links.user.js) 直接安裝腳本。
   - **方法二**：
     1. 下載本倉庫中的 `prefetch-links.user.js` 檔案。
     2. 在 Tampermonkey 中點擊「新增腳本」，然後將下載的腳本內容粘貼進去，保存即可。

## 使用方法

安裝完成後，腳本會自動在符合條件的網站上運行。當您將滑鼠移動到一個連結時，該連結的資源將被預先載入。此外，所有帶有 `download` 屬性的連結將被自動屏蔽，防止不必要的下載行為。

## 範例

以下是一個示例連結：

```html
<a href="https://example.com/page" download>下載頁面</a>
<a href="https://example.com/page2">訪問頁面</a>
