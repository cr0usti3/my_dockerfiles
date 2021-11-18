#execute ruby script


FROM alpine:3.7
WORKDIR /opt
RUN apk add ruby && rm -rf /var/lib/apk/*
COPY * /opt/
ENTRYPOINT ["/usr/bin/ruby"]

