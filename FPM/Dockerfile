FROM alpine:3.6
MAINTAINER Lorelei Aurora <iam@l5i.me>

RUN apk add --no-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing/ \
        curl \
        php7 \
        php7-ctype \
        php7-curl \
        php7-dom \
        php7-exif \
        php7-fileinfo \
        php7-fpm \
        php7-gd \
        php7-gettext \
        php7-iconv \
        php7-imap \
        php7-intl \
        php7-json \
        php7-mbstring \
        php7-mcrypt \
        php7-mysqli \
        php7-mysqlnd \
        php7-openssl \
        php7-phar \
        php7-posix \
        php7-redis \
        php7-simplexml \
        php7-libsodium \
        php7-memcached \
        php7-tokenizer \
        php7-xml \
        php7-xmlreader \
        php7-zip \
        php7-zlib \
    && echo 'extension=sodium.so' > /etc/php7/conf.d/50_libsodium.ini

COPY ./fs /

CMD ["php-fpm7"]
