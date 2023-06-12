## 14. コンテナの停止と削除
##### nginxを「停止」し、削除します。
```
docker stop nginx
docker rm nginx
```{{exec}}

## 15. コンテナイメージの一覧表示
##### ホストにダウンロードされているコンテナイメージを見てみます。
`docker images`{{exec}}

## 16. コンテナイメージの削除
##### nginxイメージを削除します。
`docker rmi nginx:latest`{{exec}}

## 17. コンテナイメージの一覧表示
##### 改めてホストにダウンロードされているコンテナイメージを見てみます。
`docker images`{{exec}}