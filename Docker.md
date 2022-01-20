docker run -v C:\MyProjects\Docker:/home/jovyan -p 8888:8888 jupyter/scipy-notebook:33add21fab64


docker exec -it b1341040231d bash

docker cp wine.data b1341040231d:/home/jovyan/wine.data

у каждого докер контейнера есть подключенная папка Volume которую видит и контейнер и система


-- следующая команда берет докерфайл из текущей директории и использует команды из нее
docker run -v C:\MyProjects\Docker:/home/jovyan -p 8888:8888 688f07d45b79

docker build .
-- -t my_tag_name -- это позволяет не копировать хэш контейнера а просто сделать команду
docker build -t my_tag_name .

-- после этой команды нужно скопировать текст sha256:d31f66ef1c89d8b3a93eda8da987cf1751c5529
и вставить сразу в docker run команду

docker run -v C:\MyProjects\Docker:/home/jovyan -p 8888:8888 sha256:d31f66ef1c89d8b3a93eda8da987cf1751c5529

--docker compose

docker-compose up

также имеет флаг --build

docker-compose up --build - при изменении в файле docker-compose полезно сделать так чтобы скачать все нужные пакеты


docker-compose build

-- команда для получения свойств контейнера
docker inspect <CONTAINER ID> 

