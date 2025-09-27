# GAS Web API
模擬実習用 GAS Web API 仕様書管理プロジェクト。

## 概要
GAS 上で稼働する API を対象として Swagger UI ドキュメントです。  
固定パスワード認証を設け、パスワードを知っているユーザーのみが閲覧可能です。

## 使用技術
- Google Apps Script（バックエンド API）
- Swagger UI（API ドキュメント表示）
- Node.js / npm（ローカルでの Swagger UI 起動）
- http-server（ローカルサーバー起動）


## ローカルでの起動手順

1. リポジトリをクローン
    ```bash
    git clone git@github.com:comvace-it-solution/swagger-gas-demo.git

    cd swagger-gas-demo
2. npm モジュールインストール
    ```bash
    npm install swagger-ui-dist
    npm install -g http-server
3. localサーバーを起動
    ```bash
    http-server -p 8000
    # もしくは
    npx http-server -p 8000
4. ブラウザでアクセス
    ```arduino
    http://127.0.0.1:8000/swagger.html
5. パスワード認証
- 表示されるプロンプトに固定パスワードを入力すると Swagger UI が表示されます。
