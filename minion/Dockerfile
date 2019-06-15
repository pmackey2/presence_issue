FROM alpine:edge

RUN apk add --no-cache dumb-init \
        salt-minion

ENTRYPOINT ["/usr/bin/dumb-init", "--"]
CMD ["salt-minion", "-l", "debug"]
