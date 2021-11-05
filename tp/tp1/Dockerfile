ARG VERSION=alpine

FROM nginx:$VERSION

ENV TIMEZONE Europe/Paris

RUN apk update && apk upgrade # && apk --update --no-cache add bash

EXPOSE 80

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
