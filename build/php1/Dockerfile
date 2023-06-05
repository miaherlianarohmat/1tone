FROM php:8.1-apache

RUN apt-get update && docker-php-ext-install mysqli pdo pdo_mysql

RUN find /var/www/html -type d -exec chmod -R 755 {} \;
RUN find /var/www/html -name "*.php" -exec chmod 755 {} \;
RUN find /var/www/html -name "*.css" -exec chmod 755 {} \;
RUN find /var/www/html -name "*.js" -exec chmod 755 {} \;
RUN chown -R root:root /var/www/html
RUN a2enmod rewrite
