FROM nginx:1.18-alpine

ENV TZ=UTC

RUN apk update && \
    apk add --update --no-cache --virtual=.build-dependencies g++

# nginx config file
COPY default.conf /etc/nginx/conf.d
COPY uwsgi_params /etc/nginx/uwsgi_params
