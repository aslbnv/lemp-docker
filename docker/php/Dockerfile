FROM php:8.3-fpm

RUN docker-php-ext-install mysqli

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

RUN pecl install xdebug \
    && docker-php-ext-enable xdebug

COPY xdebug.ini $PHP_INI_DIR/conf.d/

RUN chmod 777 .