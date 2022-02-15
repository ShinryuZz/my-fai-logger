FROM ubuntu:18.04

RUN apt-get update && \
    apt-get install -y rsyslog


COPY rsyslog-client.conf /etc/rsyslog.conf

COPY startup.sh /startup.sh
RUN chmod 744 /startup.sh
CMD ["/startup.sh"]

