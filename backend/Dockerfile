FROM python:3.8-slim-buster

RUN apt-get update && apt-get install -y git

ENV FLASK_APP=noharmapp
ENV FLASK_RUN_HOST=0.0.0.0
ENV FLASK_RUN_PORT=5000

WORKDIR /app

RUN git clone https://github.com/noharm-ai/backend /app

RUN pip install --upgrade pip
RUN pip install -r /app/requirements-prod.txt

EXPOSE 5000
ENV PORT 5000

CMD python mobile.py