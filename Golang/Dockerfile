
FROM golang:1.19-alpine

WORKDIR /app

COPY go.mod ./
COPY go.sum ./

RUN go mod download

COPY . .

COPY *.go ./

RUN go build -o /main

# Or whatever port you want to expose
EXPOSE 8000 

CMD [ "/main" ]