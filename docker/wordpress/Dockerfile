FROM wordpress:latest

RUN apt-get update && apt-get install -y \
        wget \
        unzip \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Apache に書き込み権限を与える
RUN chown -R www-data:www-data /var/www/html/

WORKDIR /var/www/html
