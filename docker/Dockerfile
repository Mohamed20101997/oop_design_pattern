FROM php:8.2-cli
RUN apt update
WORKDIR /Users/root/home

# Composer installation

RUN php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
RUN php composer-setup.php
RUN php -r "unlink('composer-setup.php');"

RUN mv composer.phar /usr/local/bin/composer
WORKDIR /user/src/myapp