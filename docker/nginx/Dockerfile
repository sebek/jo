FROM bitnami/nginx:1.16.0-ol-7-r0

WORKDIR /var/www/app

COPY src .

COPY nginx.conf /opt/bitnami/nginx/conf/nginx.conf
COPY sites /opt/bitnami/nginx/conf/sites
COPY conf.d /opt/bitnami/nginx/conf/conf.d

CMD ["nginx", "-g", "daemon off;"]

EXPOSE 8080 4433