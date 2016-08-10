FROM debian:8
MAINTAINER WillemMali

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y git salt-minion

EXPOSE 4505

ENTRYPOINT salt-minion
