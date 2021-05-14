FROM postgres:11.6
WORKDIR /db

RUN apt-get update -y 
RUN apt-get install -y git

ENV POSTGRES_USER postgres
ENV POSTGRES_DB noharm
RUN git clone https://github.com/noharm-ai/database .
RUN cp noharm-create.sql /docker-entrypoint-initdb.d
RUN cp noharm-triggers.sql /docker-entrypoint-initdb.d
RUN cp noharm-insert.sql /docker-entrypoint-initdb.d
EXPOSE 5432