# NoHarm Docker Image
A Dockerfile for building the official NoHarm docker image

## Services and Ports
 - frontend (:80)
 - backend (:5000)
 - getname-api (:443)
 - [postgres](https://hub.docker.com/_/postgres) (:5432)
 - [apache-nifi](https://github.com/noharm-ai/nifi-docker) (:8080)

## Run Docker

```
$ git clone https://github.com/noharm-ai/docker-image
$ cd docker-image
$ docker-compose up -d --build
```
