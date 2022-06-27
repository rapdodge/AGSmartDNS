FROM alpine:latest
RUN mkdir /opt/smartdns
RUN mkdir /opt/smartdns/config
RUN wget -O /opt/smartdns/smartdns "https://github.com/pymumu/smartdns/releases/latest/download/smartdns-$(uname -m)"
RUN chmod a+rx /opt/smartdns/smartdns
