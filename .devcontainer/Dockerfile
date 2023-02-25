FROM php:8.1-cli

RUN apt-get update -y && apt-get install -y git vim curl libzip-dev zip unzip

RUN docker-php-ext-install pdo pdo_mysql

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /usr/src/myapp

COPY . .

