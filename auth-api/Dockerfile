FROM golang:1.19-alpine AS builder
WORKDIR /app
COPY . .
RUN go mod tidy && go build -o auth-api

FROM alpine:latest
WORKDIR /root/
COPY --from=builder /app/auth-api .
EXPOSE 8080
CMD ["./auth-api"]
