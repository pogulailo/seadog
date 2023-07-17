FROM php:8.2-fpm-alpine

RUN docker-php-ext-install pdo pdo_mysql

RUN mv $PHP_INI_DIR/php.ini-development $PHP_INI_DIR/php.ini
COPY ./app/conf.d /usr/local/etc/php/conf.d

WORKDIR /app
