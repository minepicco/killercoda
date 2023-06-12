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

## 5. nginxを「停止」します。
##### 次のコマンドを使ってnginxコンテナを停止します。
`docker stop nginx`{{exec}}

## 6. コンテナ一覧表示
##### 次のコマンドを使って稼働中のコンテナを一覧表示します。
`docker ps`{{exec}}

##### 停止も含めた稼働中のコンテナ一覧を見てみます。
`docker ps -a`{{exec}}

## 7. 再アクセステスト
##### 再度アクセスし、ページが存在しないことを確認します。
[NGINXにアクセス]({{TRAFFIC_HOST1_80}})

## 8. コンテナの削除
##### nginxコンテナを削除します。
`docker rm nginx`{{exec}}

### 停止も含めた稼働中のコンテナ一覧を見てみます。
`docker ps -a`{{exec}}

### ホストにダウンロードされているコンテナイメージを見てみます。
`docker images`{{exec}}

### もう一度nginxをデプロイしてみます。
イメージはすでにダウンロード済みなので、起動が早いです:
`docker run --name nginx -p 80:80 -d nginx:latest`{{exec}}

### nginxにアクセスし、ウェルカムページが表示されることを確認します。
[ACCESS NGINX]({{TRAFFIC_HOST1_80}})

### 稼働中のコンテナ一覧を見てみます。
`docker ps`{{exec}}

### nginxを「停止」し、削除します。
```
docker stop nginx
docker rm nginx
```{{exec}}

### ホストにダウンロードされているコンテナイメージを見てみます。
`docker images`{{exec}}

### nginxイメージを削除します。
`docker rmi nginx:latest`{{exec}}

### ホストにダウンロードされているコンテナイメージを見てみます。
`docker images`{{exec}}