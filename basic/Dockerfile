FROM ubuntu:latest
RUN apt-get update && \
    apt-get install -y wget && \
    wget https://s3.amazonaws.com/downloads.wercker.com/cli/stable/linux_amd64/wercker -O /usr/local/bin/wercker && \
    chmod u+x /usr/local/bin/wercker
