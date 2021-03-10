FROM mariadb:10.5

COPY schema.sql /docker-entrypoint-initdb.d/
#COPY ./Csv/ /var/lib/mysql/csv
#COPY custom.cnf /etc/mysql/conf.d

RUN touch slow-queries.log
RUN chown mysql:mysql slow-queries.log

EXPOSE 3306
