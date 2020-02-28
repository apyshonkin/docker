FROM alpine:3.11.3

MAINTAINER alex@pyshonk.in

RUN apk add --no-cache squid

COPY squid.conf /etc/squid/squid.conf

VOLUME /etc/squid/.squidusers:/etc/squid/.squidusers:ro

EXPOSE 31289

CMD ["squid", "-N", "-f", "/etc/squid/squid.conf"]
