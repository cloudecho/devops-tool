FROM maven:3.8.5-jdk-11
LABEL maintainer="Yong Ma <simple163@yahoo.com>"

RUN apt-get update && \
    apt-get -y install \
      apt-transport-https \
      ca-certificates \
      curl \
      gnupg2 \
      software-properties-common

RUN curl -fsSL https://download.docker.com/linux/$(. /etc/os-release; echo "$ID")/gpg | apt-key add -

RUN add-apt-repository \
      "deb [arch=amd64] https://download.docker.com/linux/$(. /etc/os-release; echo "$ID") \
      $(lsb_release -cs) \
      stable"

RUN apt-get update && \
    apt-get -y install make docker-ce-cli