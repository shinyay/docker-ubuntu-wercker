FROM ubuntu:17.10
RUN apt-get update && \
    apt-get install -y wget git && \
    apt-get install -y software-properties-common python-software-properties debconf-utils && \
    add-apt-repository -y ppa:webupd8team/java && \
    apt-get update && \
    echo "oracle-java8-installer shared/accepted-oracle-license-v1-1 select true" | debconf-set-selections && \
    apt-get install -y oracle-java8-installer && \
    apt-get install -y oracle-java8-set-default && \
    wget https://s3.amazonaws.com/downloads.wercker.com/cli/stable/linux_amd64/wercker -O /usr/local/bin/wercker && \
    chmod u+x /usr/local/bin/wercker
