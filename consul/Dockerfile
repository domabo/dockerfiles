FROM ubuntu
MAINTAINER Domabo <admin@domabo.com>

# install dependencies
RUN apt-get update && apt-get install -y \
    wget \
    unzip

# install consul
RUN wget https://dl.bintray.com/mitchellh/consul/0.2.0_linux_amd64.zip -O /tmp/consul.zip -P /tmp/ --no-check-certificate && unzip /tmp/consul.zip -d /tmp/
RUN chmod +x /tmp/consul
RUN mv /tmp/consul /usr/bin/consul
EXPOSE 8300
