#### スペース2回で改行
#### シャープ記号で見出し（見出しのレベルはシャープの数）

### 基本コマンド
### mysqlをpull
### Python3.6をpull

# 基本コマンド
docker --version  
docker info  
docker run -d -p 8080:80 --name コンテナ名称 イメージ  
docker ps  
docker kill コンテナID  
docker rm コンテナ名称  
docker image ls (docker imagesと同じ)  
docker image inspect イメージ名  
docker image tag イメージ名 リポジトリ名:TAG  


# mysqlをpull
docker pull mysql  
docker run --name mysql -e MYSQL_ROOT_PASSWORD=mysql -d -p 3306:3306 mysql  
docker exec -it コンテナID bash  
## mysqlのコマンド  
show databases;  
show tables;

# Python3.6をpull
docker image pull python:3.6  
docker run --name python36 -i -t python3.6 /bin/bash  


