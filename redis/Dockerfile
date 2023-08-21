FROM redis:latest

LABEL org.opencontainers.image.source=https://github.com/anirv20/simple-fortune-cookie

WORKDIR /usr/src/app

EXPOSE 6379

CMD [ "redis-server", "--save 20 1 --loglevel warning --requirepass eYVX7EwVmmxKPCDmwMtyKVge8oLd2t81" ]