FROM golang:1.8-alpine3.6

COPY . /go/src/croc-hunter
COPY static/ static/

ENV GOPATH /go
RUN cd $GOPATH/src/croc-hunter && go install -v .

CMD ["croc-hunter"]

EXPOSE 8080