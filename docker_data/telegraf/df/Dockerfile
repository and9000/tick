FROM telegraf:1.3.5-alpine
MAINTAINER Andrea Lorenzetti <andrea@lorenzetti.me>

RUN apk add --no-cache python3 && \
    python3 -m ensurepip && \
    rm -r /usr/lib/python*/ensurepip && \
    pip3 install --upgrade pip setuptools && \
    if [ ! -e /usr/bin/pip ]; then ln -s pip3 /usr/bin/pip ; fi && \
    rm -r /root/.cache && \
    # Install compile deps.
    apk add --no-cache build-base python3-dev && \
    # Install python packages.
    pip3 install requests numpy
