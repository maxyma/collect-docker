From storkmax/alpine-bash

RUN apk update && \
    apk add  php7 php7-bcmath php7-curl php7-fpm php7-gmp php7-iconv php7-mbstring php7-mysqlnd php7-opcache \
        php7-pcntl php7-pdo php7-pdo_mysql php7-pecl-redis php7-simplexml php7-sodium php7-tidy php7-zip  && \
    sed -ri ' s~^(display_errors =).*$~\1 on~; s~^(display_startup_errors =).*$~\1 on~; s~^(memory_limit =).*$~\1 256M~; ' /etc/php7/php.ini && \
    sed -ri ' s~^(listen =).*$~\1 9000~ ' /etc/php7/php-fpm.d/www.conf && \
    apk add  nginx  && \
    rm -rf /var/cache/apk/*

WORKDIR /
COPY run.sh .

CMD ["sh", "/run.sh"]
