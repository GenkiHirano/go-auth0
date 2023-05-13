# Auth0

## ゴール

- Go で Auth0 で認証・認可を実装して遊ぶ

## コマンド

### JWT 取得

```shell
curl --request POST \
  --url https://kkfactory.jp.auth0.com/oauth/token \
  --header 'content-type: application/json' \
  --data '{"client_id":"XXXXXXX","client_secret":"XXXXXXX","audience":"XXXXXXX","grant_type":"client_credentials"}'
```

### サーバー起動

```shell
go run main.go
```

### API 実行

```shell
curl --request GET \
  --url http://path_to_your_api/ \
  --header 'XXXXXX'
```
