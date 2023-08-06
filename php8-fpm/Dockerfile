FROM php:8.2-fpm
RUN apt-get update && apt-get install -y \
		libfreetype-dev \
		libjpeg62-turbo-dev \
		libpng-dev \
        libzip-dev \
	&& docker-php-ext-configure gd --with-freetype --with-jpeg \
	&& docker-php-ext-install -j$(nproc) gd \
    && docker-php-ext-configure zip \
    && docker-php-ext-install -j$(nproc) zip
<<<<<<< HEAD
=======
RUN apt-get clean
>>>>>>> be60626 (adding clean at the end)
