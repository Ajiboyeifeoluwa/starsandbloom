FROM php:8.2-apache

# Install PHP extensions required for MariaDB/MySQL
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Copy the application into Apache's web root
COPY . /var/www/html/

# Set correct permissions
RUN chown -R www-data:www-data /var/www/html