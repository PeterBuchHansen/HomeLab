FROM ubuntu:noble

ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
        python3 \
        python3-venv \
        python3-pip \
        build-essential \
        curl \
        git \
        nano

RUN rm -rf /var/lib/apt/lists/*

RUN python3 -m pip install pre-commit --break-system-packages
