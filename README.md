# curso-kubernetes

docker run --name guss-mysql -e MYSQL_ROOT_PASSWORD=guss2020 -d --restart always mysql:latest

docker run --name guss-postgres -e POSTGRES_PASSWORD=guss2020 -d --restart always postgres:latest

docker exec -it guss-mysql bash
mysql -u root -pguss2020
CREATE DATABASE msvc_usuarios;
system clear
SHOW DATABASES;

docker exec -it guss-postgres bash
psql -U postgres
CREATE DATABASE msvc_cursos;
\list
\! clear

docker inspect --format '{{ .NetworkSettings.IPAddress }}' guss-postgres
docker inspect --format '{{ .NetworkSettings.IPAddress }}' guss-mysql



