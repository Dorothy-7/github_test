FROM php:8.2.12-fpm

RUN set -x \
    && apt-get update \
    && apt-get install -y libicu-dev libpng-dev libzip-dev wget zip unzip vim \
    && docker-php-ext-install bcmath exif gd intl mysqli pdo_mysql sockets zip

RUN pecl install xdebug && docker-php-ext-enable xdebug