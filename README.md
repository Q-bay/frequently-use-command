# frequently-use-command
よく使うコマンドを記載したい

## Docker

### docker-composeでサービス指定してのビルド
```
docker-compose build <service>
```

### docker-composeでサービス指定してキャッシュを使わずビルド
```
docker-compose build <service> --no-cache
```


## Java

### クリーン
```
mvn clean
```
### インストール
```
mvn install
```


## python

### docker-compose起動時にdjangoプロジェクト作成
```
docker-compose run [docker-composeのサービス名] django-admin.py startproject [作成するプロジェクト名] .
```

