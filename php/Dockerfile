FROM php:7.1-fpm

#RUN apt-get update -y && apt-get install php7.1 php7.1-cli php7.1-common php7.1-json php7.1-opcache php7.1-mysql php7.1-mbstring php7.1-mcrypt php7.1-zip
# Install required dependencies
RUN apt-get update -y && apt-get install -y libc6 libfreetype6-dev \
libgd3 libjpeg62-turbo-dev libpng12-dev libvpx1 libx11-6 libxpm4 \
zlib1g ucf libcurl4-gnutls-dev libltdl7 \
libgtk2.0-0 libgdk-pixbuf2.0-0 libfontconfig1 libxrender1 libglib2.0-0  libxft2 \
mysql-client libmagickwand-dev --no-install-recommends \
libmcrypt-dev libgcc1 libicu52 libicu-dev wget git



# Install required php extensions
RUN docker-php-ext-install gd && \
docker-php-ext-install mcrypt && \
docker-php-ext-install intl && \
docker-php-ext-install curl && \
docker-php-ext-install pdo_mysql
