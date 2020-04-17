FROM php:7.3-fpm-alpine

# Set Environment Variables
ENV DEBIAN_FRONTEND noninteractive

RUN apk update \
    && apk upgrade \
    && docker-php-ext-install \
        pdo_mysql

WORKDIR /var/www

CMD ["php-fpm"]

EXPOSE 9001