FROM bitnami/nginx:1.16.0-ol-7-r0

WORKDIR /var/www/app

COPY src .

COPY /docker/nginx/nginx.conf /opt/bitnami/nginx/conf/nginx.conf
COPY /docker/nginx/sites /opt/bitnami/nginx/conf/sites
COPY /docker/nginx/conf.d /opt/bitnami/nginx/conf/conf.d

CMD ["nginx", "-g", "daemon off;"]

EXPOSE 8080 4433