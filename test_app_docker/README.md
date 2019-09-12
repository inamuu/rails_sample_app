### セットアップ

```sh
docker-compose run rails rails new . --force --database=mysql --skip-bundle
docker-compose run rails rails db:create
docker-compose up -d
```

http://localhost:8080

### トラブルシュート

下記ファイルを消しておく。  
rails serverが起動すると下記ファイルが出来上がるので、下記ファイルがある状態でコンテナが停止すると再起動時にrails serverが起動できないため。

```sh
ls -l src/tmp/pids/server.pid
```
