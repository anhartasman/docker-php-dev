import sql file to a database

docker exec -i 4f551a4581c9 mysql -uroot -pMYSQL_ROOT_PASSWORD urun < urun.sql
 
get in to running container

docker exec -it f2c46977f7be /bin/bash

execute sql command

docker exec -i f2c46977f7be mysql -uroot -pMYSQL_ROOT_PASSWORD urun  <<< "SHOW TABLES;"

copy file from running container
docker cp 370c3598497d:/etc/apache2/apache2.conf .

docker inspect \
  -f '{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}' 370c3598497d

tutorial link
https://www.section.io/engineering-education/dockerized-php-apache-and-mysql-container-development-environment/