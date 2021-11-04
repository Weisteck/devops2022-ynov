ARG VERSION=3.13

FROM alpine:$VERSION as builder

RUN apk update && apk upgrade 

FROM nginx:alpine

ENV TIMEZONE Europe/Paris

RUN apk update && apk upgrade

# COPY --from=builder /index.html /var/www/html/index.html

EXPOSE 80

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
