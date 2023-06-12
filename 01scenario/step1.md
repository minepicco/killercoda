## 1. バージョン確認
##### dockerのバージョンを確認します。
`docker --version`{{exec}}

## 2. デプロイ
##### docker hubに公開されているnginxのオフィシャルイメージを使ってWebサーバーをデプロイします。
`docker run --name nginx -p 80:80 -d nginx:latest`{{exec}}

## 3. コンテナ一覧表示
##### 次のコマンドを使って稼働中のコンテナを一覧表示します。
`docker ps`{{exec}}

## 4. アクセステスト
##### nginxにアクセスし、ウェルカムページが表示されることを確認 します。
[NGINXにアクセス]({{TRAFFIC_HOST1_80}})
