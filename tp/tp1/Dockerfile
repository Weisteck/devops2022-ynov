# ARG VERSION=3.13

# FROM alpine:$VERSION as builder

# RUN apk update && apk upgrade && apk --update --no-cache add bash

# RUN echo "$VERSION test" > /message.txt

FROM nginx:alpine

ENV TIMEZONE Europe/Paris

RUN apk update && apk upgrade # && apk --update --no-cache add bash

# WORKDIR /opt

# COPY --from=builder /message.txt /opt/message.txt

# CMD ["cat", "/opt/message.txt"]
# ENTRYPOINT ["/usr/bin/cat", "/opt/message.txt"]

EXPOSE 80

ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
