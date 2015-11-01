
##### 準備
----
```
docker pull php:5.6-apache
docker pull php:tag
docker pull -a php
```

##### Docker Image Tag
----
+ https://hub.docker.com/_/php/
	+ 5.3.29-apache
	+ 5.4-apache
	+ 5.5-apache
	+ 5.6-apache
	+ 7.0-apache

##### 起動
----
+ 事前にDBを起動しておく
	+ ref: https://github.com/tuki0918/docker_mysql_run
```
docker run -itd -P -v $(pwd):/var/www/html --link some-mysql:db --name php5.6-apache php:5.6-apache
```
