FROM ubuntu:24.04
LABEL maintainer="hayamizu <hayamizu@kansai-u.ac.jp>"
RUN mkdir -p /cefore
WORKDIR /cefore
RUN apt update
RUN apt install -y git build-essential libssl-dev
RUN apt install -y automake
RUN apt install -y iputils-ping net-tools ifstat
RUN apt install -y emacs
RUN apt install -y python3
RUN apt -y clean
RUN git clone https://github.com/cefore/cefore.git

WORKDIR /cefore/runner_test
RUN apt -y clean
