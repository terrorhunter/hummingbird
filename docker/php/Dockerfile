FROM php:8.4-fpm

RUN apt-get update && \
    apt-get upgrade -y && \
    pecl channel-update pecl.php.net && \
    pecl install xdebug && \
    docker-php-ext-enable xdebug && \
    apt-get clean

COPY 00-xdebug.ini "${PHP_INI_DIR}/conf.d"