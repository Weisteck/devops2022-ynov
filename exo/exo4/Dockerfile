FROM nginx:alpine

ENV TIMEZONE Europe/Paris

RUN apk update && apk upgrade

EXPOSE 80

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
