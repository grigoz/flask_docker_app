FROM alpine:edge

RUN echo "http://dl-8.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories

RUN apk update && apk upgrade && apk --no-cache --update-cache add postgresql-client su-exec curl nano

COPY ./load_data.sh /home/
COPY ./hw1.sql /home/
