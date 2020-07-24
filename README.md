# Skillup 課題

## Version

-   Laravel 6.18.26
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

## 環境の再構築

php コンテナに入る

```
$ docker-compose exec app bash
```

composer のインストール

```
$ composer install
```

.env ファイルのコピー

```
$ cp .env.example .env
```

key:generate の生成

```
$ php artisan key:generate
```

マイグレーションの実行

```
$ php artisan migrate
```

## URL

Laravel ウェルカム画面の表示 http://localhost:9000

phpmyadmin http://localhost:3000

## データベース

データベースは以下の通り

```
CONNECTION=mysql
HOST=mysql
PORT=3306
DATABASE=docker_db
USERNAME=docker
PASSWORD=docker
```
