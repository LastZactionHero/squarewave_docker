FROM golang:1.6

RUN apt-get update -qq

ADD ./src /go/src/github.com/LastZactionHero/contact_us/
WORKDIR /go/src/github.com/LastZactionHero/contact_us/

RUN go get -d -v
