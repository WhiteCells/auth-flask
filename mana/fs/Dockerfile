FROM golang:1.23-alpine

WORKDIR /app/backend

COPY . .

RUN go mod tidy

EXPOSE 8080

CMD ["go", "run", "main.go", "--address=0.0.0.0"]
