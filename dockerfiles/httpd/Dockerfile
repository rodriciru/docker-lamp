FROM httpd:alpine

RUN apk update \
    && apk add certbot \
    && apk add certbot-apache 

RUN apk add tzdata \ 
    && cp /usr/share/zoneinfo/Europe/Madrid /etc/localtime \
    && echo "Europe/Madrid" >  /etc/timezone