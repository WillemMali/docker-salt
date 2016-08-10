FROM debian:8
MAINTAINER WillemMali

RUN [ ! -d /etc/salt/minion.d ] && mkdir -p /etc/salt/minion.d
ADD ./master /etc/salt/minion

CMD apt-get update
CMD apt-get upgrade -y
CMD apt-get install -y git salt-master

EXPOSE 4505

ENTRYPOINT salt-master
