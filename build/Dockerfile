FROM golang:1.22.5-alpine

RUN apk update && apk add git

WORKDIR /go/src/app

COPY . .

RUN go install github.com/air-verse/air@latest \
    && go mod tidy

CMD ["air"]
