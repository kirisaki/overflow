FROM debian:stretch
MAINTAINER Akihito KIRISAKI

RUN apt update && apt install curl -y

RUN curl -sSL https://get.haskellstack.org/ | sh
ENV PATH $PATH:/root/.local/bin
RUN stack --resolver lts-13.15 setup
RUN stack install hlint stylish-haskell alex happy
