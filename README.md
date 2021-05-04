#### スペース 2 回で改行

#### シャープ記号で見出し（見出しのレベルはシャープの数）

### 基本コマンド

### mysql を pull

### Python3.6 を pull

# 基本コマンド

docker --version  
docker info  
docker run  
docker ps  
docker kill コンテナ ID  
docker rm コンテナ名称  
docker image ls (docker images と同じ)  
docker image inspect イメージ名  
docker image tag イメージ名 リポジトリ名:TAG

# docker run

オプション
--interactive 対話モード  
--tty テレタイプ
--detach バックグラウンドで起動
--p ホスト OS のポート番号:ゲスト OS のポート番号
--volume {pass}
--name {コンテナ名}

docker run -itd -p ホストポート:ゲストポート -v {ホストの pass}:{ゲストの pass} --name {コンテナ名} {イメージ名}

# mysql を pull

docker pull mysql  
docker run --name mysql -e MYSQL_ROOT_PASSWORD=mysql -d -p 3306:3306 mysql  
docker exec -it コンテナ ID bash

## mysql のコマンド

show databases;  
show tables;

# Python3.6 を pull

docker image pull python:3.6  
docker run --name python36 -i -t python3.6 /bin/bash
