FROM debian:stretch-slim

RUN set -xe \
    && apt-get update && apt-get install -y curl apt-transport-https gnupg \
    && echo "deb https://apt.cozy.io/debian/ stretch testing" > /etc/apt/sources.list.d/cozy.list \
    && curl https://apt.cozy.io/cozy.gpg | apt-key --keyring /etc/apt/trusted.gpg.d/cozy.gpg add - \
    && apt-get update && apt-get clean && apt-get autoremove

