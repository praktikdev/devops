FROM golang:latest

RUN mkdir /app 
ADD . /app/ 
WORKDIR /app

RUN go get github.com/gorilla/mux
RUN go get gopkg.in/natefinch/lumberjack.v2
RUN go build -o main . 

EXPOSE 8080

CMD ["/app/main"]