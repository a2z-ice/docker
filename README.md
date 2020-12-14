# mysql-docker

docker run --detach --name=mysql_5_7 --restart=always --volume=/home/assad/mysql-data:/var/lib/mysql -p 52001:3306  --env="MYSQL_ROOT_PASSWORD=123456" mysql:5.7
