# fastapi-todo-app-demo
[FastAPI](https://github.com/tiangolo/fastapi)でシンプルなTODOアプリのAPIを作るデモ

## Setup
PostgreSQLを起動する

```sh
docker compose up -d
```

マイグレーションを実行する

```sh
cd db
alembic upgrade head
```

FastAPIサーバーを起動する
```sh
cd ..
uvicorn app.main:app --reload
```
