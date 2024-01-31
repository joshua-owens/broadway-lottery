FROM golang:1.21

WORKDIR /usr/src/discord

COPY go.mod ./
# RUN go mod download && go mod verify

copy ./cmd/discord/ .
RUN go build -v -o /usr/local/bin/discord ./...

CMD ["discord"]