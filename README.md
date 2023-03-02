# mysql-docker
```bash
docker run --detach --name=mysql_5_7 --restart=always --volume=/home/assad/mysql-data:/var/lib/mysql -p 52001:3306  --env="MYSQL_ROOT_PASSWORD=123456" mysql:5.7
```
#Postgres docker run
```bash
docker run -d \
	--name db-postgres \
	-e POSTGRES_PASSWORD=123456 \
	-e PGDATA=/var/lib/postgresql/data/pgdata \
	-v /c/Users/DELL/postgres/data:/var/lib/postgresql/data \
	-p 5432:5432 postgres
	
```

