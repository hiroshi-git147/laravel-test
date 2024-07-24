# test1
# 環境復元方法
# gitignoreで.envファイルをバージョン管理から除外されているため
# 以下のファイルをコピー
# dockerの.env
% cp .env.example .env
# laravelの.env
% cp src/.env.example src/.env

# docker起動
docker compose up -d
 
# 一回立ち上げただけでライブラリがうまくインストールできないカモなのでdocker停止して再度起動
docker compose down

# Laravelが動作するためには必須のライブラリ群もgitignoreで除外されているため
# 再度インストールする

docker compose exec app composer install
