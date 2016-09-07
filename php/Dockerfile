FROM php:fpm
RUN apt-get update && apt-get install -y libcurl4-gnutls-dev curl libmcrypt-dev zip unzip postgresql-server-dev-all
RUN docker-php-ext-install mbstring pdo_mysql tokenizer mcrypt pdo_pgsql
RUN usermod  -u 1000 www-data
RUN groupmod -g 1000 www-data

CMD ["php-fpm"]