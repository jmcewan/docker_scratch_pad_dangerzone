FROM alpine:3.1
RUN apk add --update redis && rm -rf /var/cache/apk/* && mkdir /data && chown -R redis:redis /data && echo -e "include /etc/redis-local.conf/n" >> /etc/redis.conf

ADD root /

VOLUME["/data"]

EXPOSE 6379
