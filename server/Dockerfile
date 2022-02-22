FROM ubuntu:18.04

RUN ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apt-get update && \
    apt-get install -y rsyslog


COPY rsyslog-server.conf /etc/rsyslog.conf

COPY startup.sh /startup.sh
RUN chmod 744 /startup.sh

# CMD ["/startup.sh"]

