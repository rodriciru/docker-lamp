FROM php:7.4-fpm-alpine

RUN docker-php-ext-install mysqli
RUN apk update \
    && apk add libzip-dev \
    && apk add zlib-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install zip \
    && docker-php-ext-install pdo_mysql

RUN apk add tzdata \ 
    && cp /usr/share/zoneinfo/Europe/Madrid /etc/localtime \
    && echo "Europe/Madrid" >  /etc/timezone