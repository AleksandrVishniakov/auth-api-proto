FROM golang:1.26.5-alpine

RUN apk -U upgrade && \
    apk add bash git go-task protoc

RUN go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.36.6 && \
    go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.5.1 && \
    go install github.com/envoyproxy/protoc-gen-validate@v1.2.1 && \
    go install github.com/easyp-tech/easyp/cmd/easyp@latest
