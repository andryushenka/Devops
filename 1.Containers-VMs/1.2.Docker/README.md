# Работа с Docker
### 2.6.2 Устанавливаем Docker на машину и выполняем проверку
![hello-world](images/install.png)

### 2.6.3 Скачаем контейнер с nginx и запустим с парметром -p
```
docker pull nginx
docker run --name (my-nginx) -p 8080:80 nginx
```
![nginx](images/nginx%20install.png)
![run nginx](images/run%20nginx.png)
![](images/host.png)

### 2.6.4 Запустим контейнер с MySQL используя -v
```
docker pull mysql
docker run --name my-mysql -v /my/own/datadir: /var/lib/mysql -e MYSQL_ROOT_PASSWORD=(qwert) mysql
```
![mysql](images/mysql%20run.png)

### 2.6.5 Подключимся к базе, создадим нового пользователя и базу
```
Запустим командную строку в контейнере:

docker exec -it mysql /bin/bash


>mysql -u root -p
>CREATE USER ''@'localhost' IDENTIFIED BY ''
>CREATE DATABASE ''
```
![](images/DATABASE0.png)
![](images/DATABASE.png)
 
# Работа с Dockerfile

### Создать образ с Ubuntu 20.04 и Ruby 2.7.2
![](/images/RUBY%20-v.png)

# Работа с Docker-compose
![](images/wordpr0.png)
![](/images/wordpr.png)
