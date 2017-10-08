FROM mysql:5.7.19
ARG MYSQL_USER=ghost
ENV MYSQL_USER=$MYSQL_USER
COPY ./init.sql /docker-entrypoint-initdb.d
RUN echo "MYSQL_USER=$MYSQL_USER"
RUN sed -i 's/MYSQL_USER/'$MYSQL_USER'/g' /docker-entrypoint-initdb.d/init.sql
EXPOSE 3306