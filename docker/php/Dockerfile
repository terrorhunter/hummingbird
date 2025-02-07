FROM php:8.4-fpm

RUN apt-get update && \
    apt-get upgrade -y && \
    pecl channel-update pecl.php.net && \
    pecl install xdebug && \
    docker-php-ext-enable xdebug \

