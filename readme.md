# Урок и ДЗ Базы данных. JDBC

### Задачи

В проекте, который рассматривался на уроке необходимо дописать код так, чтобы все тесты стали зелеными.
Проект написан на Java поэтому:

- установить JDK Java на машину
- нужно установить нужно установить специальную IDE InteligenIdea

### Настройки Postgres

контейнер postgres = my-postgres  
POSTGRES_PASSWORD=password
POSTGRES_USER=user  
название базы данных POSTGRES_DB=productStar

### Команды Postgres

`docker run -d -p 5435:5432 --name my-postgres -e POSTGRES_PASSWORD=password -e POSTGRES_USER=user -e POSTGRES_DB=productStar postgres`
-запуск контейнера с указанным образом в фоновом режиме и маппингом портов  
` psql -h localhost -p 5435 -U user -d productStar` - запуск контейнера PostgreSQL в фоновом режиме и подключения к
нему. !!!Если
контейнер ранее был создан, то сначало нужно удалить его.
`docker rm -f <указать id>`- удаление контейнера. Флаг -f означает принудительно удалить работающий контейнер (
использует SIGKILL)
Пример `docker rm -f d7701fb47d094e549c9d4f6eac51db85a023f433312034d5b619318c5e151e34`
`docker ps` - проверка в консоли что контейнер запущен






