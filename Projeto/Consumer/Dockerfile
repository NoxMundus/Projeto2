FROM python:3.8-alpine

RUN pip install --upgrade pip
RUN pip install pika
RUN pip install redis

RUN apk add --update gcc
RUN apk add musl-dev
RUN apk add libc-dev
RUN apk add libffi-dev

RUN pip install minio

WORKDIR /app
COPY Consumertest.py .

CMD python3 -u /app/Consumertest.py
#ENTRYPOINT python3 Consumertest.py
