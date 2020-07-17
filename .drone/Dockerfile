FROM alpine:3.12
RUN apk add -U --no-cache ca-certificates

WORKDIR /data
ENV HOME=/data
COPY ./build/gaiad /usr/bin/gaiad
COPY ./build/gaiacli /usr/bin/gaiacli
EXPOSE 26657

CMD ["gaiad", "start", "--pruning", "nothing"]
