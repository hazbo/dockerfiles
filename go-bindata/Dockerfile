# go-bindata in a container
#
# docker run --rm \
#   -v $(pwd):/home \
#   hazbo/go-bindata
#

FROM golang:1.6-alpine
MAINTAINER Harry Lawrence

RUN apk update && apk add \
        git \
        && rm -rf /var/cache/apk/*

RUN go get -u github.com/jteeuwen/go-bindata/...

WORKDIR /home

CMD [ "go-bindata" ]

