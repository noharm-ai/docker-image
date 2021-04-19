FROM postgres:11.6
WORKDIR /
ENV POSTGRES_USER postgres
#ENV POSTGRES_PASSWORD postgres
ENV POSTGRES_DB noharm
COPY database/noharm-create.sql /docker-entrypoint-initdb.d
COPY database/noharm-triggers.sql /docker-entrypoint-initdb.d
COPY database/noharm-insert.sql /docker-entrypoint-initdb.d
EXPOSE 5432