1. 如果跳出淘寶的資訊不小心按到 enter，解決方法要去開 一個檔案裏面新增 ...:false
2. 開啟資料夾直接開成根目錄，不然 eslint 不會幫你修錯誤
(共用 vscode 連結在 Y 槽)
3. scripts 需重設
windows:
    "serve": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service serve",
    "build": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service build",
    "lint": "SET NODE_OPTIONS=--openssl-legacy-provider && vue-cli-service lint",

mac:
    "serve-linux": "SET NODE_OPTIONS=--openssl-legacy-provider; vue-cli-service serve",
    "build-linux": "SET NODE_OPTIONS=--openssl-legacy-provider; vue-cli-service serve",
    "lint-linux": "SET NODE_OPTIONS=--openssl-legacy-provider; vue-cli-service serve"

4. npm i -D pug pug-plain-loader
5. npm run serve
6. 沒事檔案不要放 public 資料夾，他是靜態資源，涉及打包問題


1. html 只有一層，老樣子
2. assets 、 components 內的東西清空
3. format on save 要改成 false
4. 