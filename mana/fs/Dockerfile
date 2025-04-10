FROM golang:1.23-alpine AS build

WORKDIR /app/backend

COPY go.mod go.sum ./

RUN go mod tidy

COPY . .

RUN go build -o app .

FROM alpine:latest

RUN apk add --no-cache libc6-compat

WORKDIR /app

COPY --from=build /app/backend/app /app/

EXPOSE 8080

CMD ["./app", "--address=0.0.0.0"]
