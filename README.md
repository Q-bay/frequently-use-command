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

### ymlに紐ついているコンテナとイメージの削除
```
docker-compose down --rmi all --volumes --remove-orphans
```

### docker不要イメージの削除
```
docker image prune
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

### テストスキップ
```
mvn install -Dmaven.test.skip=true
```


## Python

### docker-compose起動時にdjangoプロジェクト作成
```
docker-compose run [docker-composeのサービス名] django-admin.py startproject [作成するプロジェクト名] .
```

## postgres
### ログイン(-h:ホスト -U:user -p:ポート)
```
psql -h localhost -U postgres -p 5432 
```
## React
### プロジェクト作成
npx create-react-app <プロジェクト作成> --template <テンプレート(typescriptとか)>

### 起動
npm start

## TypeScript
### コンパイル
npx tsc

### 実行
npx ts-node app.ts


## Go
### 環境変数の設定
go env -w GOPATH=HOGE

