FROM alpine
RUN apk add --update \
    python \
    python-dev \
    py-pip
RUN apk update
RUN apk add ca-certificates 
RUN apk add openssl
RUN update-ca-certificates
RUN apk add --update bash && rm -rf /var/cache/apk/*
RUN wget https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-113.0.0-linux-x86_64.tar.gz
RUN tar -xvf google-cloud-sdk-113.0.0-linux-x86_64.tar.gz
RUN ./google-cloud-sdk/install.sh

