FROM golang

WORKDIR /go

RUN go get github.com/gorilla/mux

RUN go get github.com/urfave/negroni

ADD . /go/src/github.com/tobyjsullivan/lunch-n-learn

WORKDIR /go/src/github.com/tobyjsullivan/lunch-n-learn

RUN go install github.com/tobyjsullivan/lunch-n-learn

EXPOSE 3000

CMD /go/bin/lunch-n-learn


