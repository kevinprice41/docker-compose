FROM alpine:3.4
RUN apk --no-cache add dnsmasq
RUN echo "conf-dir=/etc/dnsmasq.d/,*.conf" >> /etc/dnsmasq.conf
COPY price.conf /etc/dnsmasq.d/price.conf
EXPOSE 53 53/udp
CMD ["dnsmasq", "-k"]
