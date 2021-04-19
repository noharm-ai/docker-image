FROM postgres:11.6
WORKDIR /
ENV POSTGRES_USER postgres
#ENV POSTGRES_PASSWORD postgres
ENV POSTGRES_DB noharm
COPY noharm-create.sql /docker-entrypoint-initdb.d
COPY noharm-triggers.sql /docker-entrypoint-initdb.d
COPY noharm-insert.sql /docker-entrypoint-initdb.d
EXPOSE 5432