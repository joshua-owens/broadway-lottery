FROM golang:1.21

WORKDIR /usr/src/scraper

COPY go.mod ./
# RUN go mod download && go mod verify

copy ./cmd/scraper/ .
RUN go build -v -o /usr/local/bin/scraper ./...

CMD ["scraper"]