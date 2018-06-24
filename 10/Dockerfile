FROM node:10.5.0
MAINTAINER Lowie Huyghe <iam@lowiehuyghe.com>

# Config
ENV GOOGLE_CLOUD_SDK_VERSION 206.0.0

# Files
COPY files/get-gae-version /usr/local/bin/


# Google Cloud SDK
RUN wget --quiet --output-document=/opt/google-cloud-sdk.tar.gz https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-${GOOGLE_CLOUD_SDK_VERSION}-linux-x86_64.tar.gz
RUN tar -xzf /opt/google-cloud-sdk.tar.gz -C /opt \
    && rm -rf /opt/google-cloud-sdk.tar.gz
RUN /opt/google-cloud-sdk/install.sh
ENV PATH="${PATH}:/opt/google-cloud-sdk/bin"
