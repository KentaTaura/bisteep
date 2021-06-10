# bisteep

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).  
  
<br><br>

# Firebaseへのデプロイ方法
https://console.firebase.google.com/  

## バージョンの確認
```bash
$ firebase -V (キャピタル V)
```

## Firebase にログイン
```bash
$ firebase login
```
## Firebase をログアウト
```bash
$ firebase logout
```  
firebase projects:list と firebase deploy　でエラーが出る場合は、ログインし直す  


## ローカルでテスト
http://localhost:5000/ でローカルファイルがブラウザで確認できる。
dist配下のファイル(deployするファイル)でテストできるので、`npm run dev` のローカル開発環境とは異なる

```bash
$ firebase emulators:start
```

## デプロイ
デプロイする前に必ず、`npm run generate` すること！！
```bash
$ firebase deploy
```
今いるブランチのdistファイルがアップされる
