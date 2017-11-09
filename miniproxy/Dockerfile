FROM php

RUN mkdir -p /var/www/mp
ADD index.php /var/www/mp
EXPOSE 80
WORKDIR /var/www/
ENTRYPOINT ["php", "-S", "0.0.0.0:80"]
