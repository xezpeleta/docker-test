ARG BUILD_VERSION
FROM test/build:${BUILD_VERSION} as build
FROM ubuntu as base

COPY --from=build /app /app

RUN apt-get update && apt-get install --assume-yes --no-install-recommends cowsay \
    && rm -rf /var/lib/apt/lists/* 

ENV PATH $PATH:/usr/games
CMD cat /app/hello.txt | cowsay
