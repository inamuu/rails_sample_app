### setup

```sh
docker-compose run rails rails new . --force --database=mysql --skip-bundle
docker-compose run rails rails db:create
docker-compose up -d
```

http://localhost:8080


