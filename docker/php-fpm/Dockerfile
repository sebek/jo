FROM bitnami/php-fpm:7.1.30

RUN chgrp -R 0 /opt/bitnami/php/var && chmod -R g=u /opt/bitnami/php/var
RUN chgrp -R 0 /opt/bitnami/php/tmp && chmod -R g=u /opt/bitnami/php/tmp
RUN chgrp -R 0 /opt/bitnami/php/logs && chmod -R g=u /opt/bitnami/php/logs

WORKDIR /var/www/app

COPY src .

CMD ["php-fpm"]

EXPOSE 9000