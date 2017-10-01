FROM golang:1.9-alpine

ADD . /go/src/github.com/0xbd31/MinnanoProxy/test/simpleserver

RUN go install github.com/0xbd31/MinnanoProxy/test/simpleserver

# Load web content into /var/www/html directory
RUN mv /go/src/github.com/0xbd31/MinnanoProxy/test/simpleserver/www /var

ENTRYPOINT /go/bin/simpleserver

EXPOSE 8080