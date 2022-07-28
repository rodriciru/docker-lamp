FROM phpmyadmin:5-fpm-alpine
    
RUN apk add tzdata \ 
    && cp /usr/share/zoneinfo/Europe/Madrid /etc/localtime \
    && echo "Europe/Madrid" >  /etc/timezone