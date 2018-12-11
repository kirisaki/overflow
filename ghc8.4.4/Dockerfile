FROM debian:9.6-slim
MAINTAINER Akihito KIRISAKI

RUN apt update && apt install curl -y
RUN curl -sSL https://get.haskellstack.org/ | sh
ENV PATH $PATH:/root/.local/bin
RUN stack --resolver lts-12.20 setup
RUN stack install hlint stylish-haskell
