FROM php:fpm-alpine
LABEL maintainer="dummymail@gmail.com"
RUN docker-php-ext-install pdo_mysql mysqli
COPY confs/php.ini /usr/local/etc/php
