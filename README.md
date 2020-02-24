### スペース2回で改行
### シャープ記号で見出し（見出しのレベルはシャープの数）


# 基本コマンド
docker --version  
docker info  
docker run -d -p 8080:80 --name コンテナ名称 イメージ  
docker ps  
docker kill コンテナID  
docker rm コンテナ名称  

# mysqlをpull
docker pull mysql  
docker run --name mysql -e MYSQL_ROOT_PASSWORD=mysql -d -p 3306:3306 mysql  
docker exec -it コンテナID bash  
## mysqlのコマンド  
show databases;  
show tables;
