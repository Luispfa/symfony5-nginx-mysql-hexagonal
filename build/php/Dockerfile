FROM php:8.0-fpm

RUN apt-get update && apt-get install -y

RUN apt-get update && apt-get install -y --no-install-recommends \
    git \
    zlib1g-dev \
    libxml2-dev \
    libzip-dev \
    zip \
    && docker-php-ext-install zip \
    intl \
    mysqli \
    pdo pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php && mv composer.phar /usr/local/bin/composer

WORKDIR /var/www/sf5
    
