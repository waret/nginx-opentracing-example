FROM golang:1.12.9-stretch

WORKDIR /app
ADD . /app
RUN go build -o /app/server server.go

EXPOSE 9001
CMD ["/app/server", "-collector_host", "jaeger", "-collector_port", "6831"]
