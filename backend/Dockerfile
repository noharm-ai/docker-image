FROM python:3.8-slim-buster
WORKDIR /app

RUN apt-get update -y 
RUN apt-get install -y git

RUN git clone https://github.com/noharm-ai/backend .
RUN pip install -r requirements.txt
COPY config.py .
EXPOSE 5000
CMD [ "python3", "mobile.py"]