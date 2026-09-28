FROM golang:1.27-alpine

WORKDIR /app

COPY ./dispatcher.go ./

RUN go build -o dispatcher ./dispatcher.go

COPY ./static ./static

CMD ["./dispatcher", "-port", "80"]