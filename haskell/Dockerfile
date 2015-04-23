FROM ubuntu:trusty

ENV LANG C.UTF-8

RUN apt-get update && \
    apt-get install -y software-properties-common && \
    add-apt-repository -y ppa:hvr/ghc && \
    rm -rf /var/lib/apt/lists/*
