FROM php:8.2-apache

RUN apt-get clean
RUN apt-get update -y

RUN apt-get install -y libzip-dev zip libpng-dev

RUN docker-php-ext-install mysqli zip gd sockets

RUN a2enmod rewrite && a2enmod headers
