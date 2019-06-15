FROM alpine:edge

EXPOSE 4505/tcp
EXPOSE 4506/tcp

RUN apk add --no-cache dumb-init \
        py3-redis \
        salt-master

ENTRYPOINT ["/usr/bin/dumb-init", "--"]
CMD ["salt-master", "-l", "debug"]
