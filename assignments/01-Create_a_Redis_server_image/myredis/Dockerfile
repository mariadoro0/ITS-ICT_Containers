FROM ubuntu:latest
EXPOSE 6380/tcp
RUN apt update && apt install -y redis-server
COPY redis.conf /etc/redis/redis.conf
USER redis:redis
LABEL MANTEINER="Maria Doro"
ENTRYPOINT redis-server /etc/redis/redis.conf