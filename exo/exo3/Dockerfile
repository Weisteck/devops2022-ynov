ARG VERSION=3.13

FROM alpine:$VERSION as builder

ARG VERSION

RUN apk update && apk upgrade && apk --update --no-cache add bash

RUN echo "$VERSION Test" > /message.txt

FROM alpine:$VERSION

WORKDIR /opt

COPY --from=builder /message.txt /opt/new-message.txt

CMD ["cat", "/opt/new-message.txt"]
