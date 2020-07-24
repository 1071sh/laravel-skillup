# 自由課題

## Version

-   nginx
-   php:7.4-fpm-buster
-   mysql
-   phpmyadmin

## 起動・停止

起動

```
$ docker-compose up -d
```

停止

```
$ docker-compose down
```

app コンテナに入る

```
$ docker-compose exec app bash
```

mysql コンテナに入る

```
$ docker exec -it mysql bash
```

mysql に接続

```
mysql -u root -p
```

## URL

Laravel ウェルカム画面の表示　http://localhost:9000
phpmyadmin http://localhost:3000

## データベース

データベースは以下の通り

```
CONNECTION=mysql
HOST=127.0.0.1
PORT=3306
DATABASE=docker_db
USERNAME=docker
PASSWORD=docker
```
