# Alpine-Linux + nginx + php7-fpm + mysql + ssh + s6-overlay 
[![](https://images.microbadger.com/badges/image/jmaciasportela/alpine-s6-nginx-php7-mysql-ssh.svg)](https://microbadger.com/images/jmaciasportela/alpine-s6-nginx-php7-mysql-ssh "Get your own image badge on microbadger.com")
[![](https://images.microbadger.com/badges/version/jmaciasportela/alpine-s6-nginx-php7-mysql-ssh.svg)](https://microbadger.com/images/jmaciasportela/alpine-s6-nginx-php7-mysql-ssh "Get your own version badge on microbadger.com")
## Usage

Available options injected as environment variable

MYSQL_PASS="Password"

Build image

sudo docker build -t "alpine-nginx-php7-mysql-ssh" .

Start the Docker container:

sudo docker run -t -i -d -p 8080:80 -p 2022:22 -v your_php:/var/www/html -e "MYSQL_PASS=password" --name=cool_container jmaciasportela/alpine-nginx-php7-mysql-ssh

Open http://localhost:8080 on your browser

## Including
 
 - NGINX 1.* (latest pkgs version)
 - PHP 7.* (latest pkgs version)
 - MySQL (latest pkgs version)
 - composer (/usr/local/bin/composer)
 - curl
 - bash
 - sshd

## PHP 7 Modules

 - php7-fpm 
 - php7-xml 
 - php7-xsl 
 - php7-pdo 
 - php7-pdo_mysql 
 - php7-mcrypt 
 - php7-curl 
 - php7-json 
 - php7-fpm 
 - php7-phar 
 - php7-openssl 
 - php7-mysqli 
 - php7-ctype 
 - php7-opcache 
 - php7-mbstring 
 - php7-session 
 - php7-pdo_sqlite 
 - php7-sqlite3 
 - php7-pcntl 
 - php7-ldap 
 - php7-soap 
 - php7-gd
 - php7-zip 
 - php7-zlib 
 - php7-xmlreader

 ## SSH

 	user: root
 	pass: root

 	To use another password, change it on Dockerfile and rebuild the image

 ## Credits

- https://github.com/smebberson/docker-alpine
- https://github.com/just-containers/base-alpine
- https://github.com/bytepark/alpine-nginx-php7
