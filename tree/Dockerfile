# tree in a container
#
# docker run --rm \
#   -v $(pwd):/home \
#   hazbo/tree
#
FROM alpine:latest
MAINTAINER Harry Lawrence

RUN apk update && apk add \
        tree \
        && rm -rf /var/cache/apk/*

WORKDIR /home

ENTRYPOINT [ "tree" ]

