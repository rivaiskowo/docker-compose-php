FROM php:5.6-apache

RUN sed -i -e 's/deb.debian.org/archive.debian.org/g' /etc/apt/sources.list
RUN sed -i -e 's|security.debian.org|archive.debian.org/|g' /etc/apt/sources.list
RUN sed -i -e '/stretch-updates/d' /etc/apt/sources.list

RUN apt-get clean
RUN apt-get update

RUN apt-get install -y libzip-dev zip libpng-dev mcrypt libmcrypt-dev libfreetype6 libfreetype6-dev libpng-dev libjpeg62-turbo libjpeg62-turbo-dev

RUN docker-php-ext-configure zip --with-libzip

RUN docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/

RUN docker-php-ext-install mysqli zip gd sockets mcrypt

RUN a2enmod rewrite && a2enmod headers
