FROM php:7.1-alpine

RUN apk add --update wget
RUN wget http://deployer.org/deployer.phar && \
    mv deployer.phar /usr/local/bin/dep && \
    chmod +x /usr/local/bin/dep && \
    apk del wget && \
    rm -rf /var/cache/apk/*

WORKDIR /app
ENTRYPOINT ["/usr/local/bin/dep"]
