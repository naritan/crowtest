FROM alpine:3.4

WORKDIR /home

RUN apk --update add --no-cache make cmake gcc libc-dev g++ boost-dev
COPY ./app .

RUN cmake .
RUN make

EXPOSE 8080
CMD ["./main"]