FROM php:7.1-apache

RUN apt-get update \
 && docker-php-ext-install pdo pdo_mysql zip \
 && a2enmod rewrite \
 && curl -sS https://getcomposer.org/installer \
  | php -- --install-dir=/usr/local/bin --filename=composer

WORKDIR /var/www/html