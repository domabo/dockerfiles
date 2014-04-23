FROM ubuntu
MAINTAINER Domabo <admin@domabo.com>

# install dependencies
RUN apt-get update && apt-get install -y \
    wget \
    unzip

# install consul
RUN wget https://dl.bintray.com/mitchellh/consul/0.1.0_linux_amd64.zip -O consul.zip -P /tmp/ --no-check-certificate && unzip /tmp/consul.zip -d /tmp/
RUN chmod +x /tmp/consul
RUN mv /tmp/consul /usr/bin/consul