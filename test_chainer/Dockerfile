FROM ubuntu:16.04

RUN apt-get update -y && \
    apt-get install -y --no-install-recommends \
    python3-dev \
    python3-tk \
    python3-pip && \
    rm -rf /var/lib/apt/lists/* /var/cache/apt/archives/*

RUN pip3 install -U setuptools

RUN pip3 install chainer
RUN pip3 install numpy matplotlib

WORKDIR "/home/workplace"

CMD /bin/bash
