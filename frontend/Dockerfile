FROM golang:1.20

LABEL org.opencontainers.image.source=https://github.com/anirv20/simple-fortune-cookie

WORKDIR /usr/src/app

# pre-copy/cache go.mod for pre-downloading dependencies and only redownloading them in subsequent builds if they change
COPY go.mod ./
RUN go mod download && go mod verify

COPY . .

RUN go build .

EXPOSE 8080

CMD ["go", "run", "frontend"]