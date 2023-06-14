# webapp-template-repo

web アプリ作成テンプレート

# 使用方法

1. Next テンプレートリポジトリからリポジトリを作成

   `https://github.com/nagata-ichiko/next-lean-repo`

1. Nest テンプレートリポジトリからリポジトリを作成

   `https://github.com/nagata-ichiko/nest-lean-repo`

1. 本テンプレートリポジトリからリポジトリを作成

1. git module をテンプレートから新たに作成したリポジトリに置き換える

1. 作成したリポジトリに合わせ、設定を変更する。

# クローン方法

` git clone --recursive https://github.com/nagata-ichiko/next-nest-learn-repo.git`

# 実行方法

- 起動
  `docker compose up`

# DB ドキュメント出力

`docker-compose up schemaspy`

# テスト実行方法

`docker-compose up api-test`

# storybook 起動方法

`docker-compose up -d storybook`

# swagger の mock サーバー立ち上げ方法

`docker-compose up -d swagger-api`

# migration 方法

## migration ファイル作成&migration

`docker-compose run --rm api npx prisma migrate dev --name ファイル名`

## うまく動かなくなったらリセット（シードファイルも一緒に入る）

`docker-compose run --rm api npx prisma migrate reset`

## seed ファイル実行(初期データ)

`docker-compose run --rm api npx prisma db seed`

# DB 確認方法

`npx prisma studio`
