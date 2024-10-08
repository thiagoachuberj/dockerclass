# dockerclass

### create container postgres
docker container run -d --name cursodocker-postgres -p 5432:5432 -e POSTGRES_PASSWORD=docker_pwd -e POSTGRES_USER=docker_usr -e POSTGRES_DB=curso_docker postgres:12-bullseye

### create container mysql
docker container run -d --name cursodocker-mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root123 -e MYSQL_DATABASE=docker_db -e MYSQL_USER=docker_usr -e MYSQL_PASSWORD=docker_pwd mysql:8.0.23

### create container mysql
docker container run -d --name cursodocker-mongo -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=mongo_usr -e MONGO_INITDB_ROOT_PASSWORD=mongo_pwd mongo:latest
