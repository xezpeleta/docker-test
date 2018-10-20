FROM alpine

ARG BUILD_VERSION=0.6
RUN mkdir /app \
    && touch /app/hello.txt \
    && echo "hello" > /app/hello.txt \
    && echo "Build version: ${BUILD_VERSION}" > /app/hello.txt
