FROM php:7.4-apache
RUN apt update && apt-get update && \
    apt install -y libmagickwand-dev imagemagick && \
    echo "" | pecl install imagick && \
    docker-php-ext-enable imagick.so && \
    docker-php-ext-install exif gd mysqli sockets
