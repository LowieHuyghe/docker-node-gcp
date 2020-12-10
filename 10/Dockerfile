FROM node:10.23.0-alpine3.11
MAINTAINER Lowie Huyghe <iam@lowiehuyghe.com>

# Config
ENV GOOGLE_CLOUD_SDK_VERSION 320.0.0

# Files
COPY files/get-gae-version /usr/local/bin/


# Google Cloud SDK
ENV PATH="/opt/google-cloud-sdk/bin:${PATH}"
RUN apk add --no-cache python3 \
  && wget --quiet --output-document=/opt/google-cloud-sdk.tar.gz https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-${GOOGLE_CLOUD_SDK_VERSION}-linux-x86_64.tar.gz \
  && tar -xzf /opt/google-cloud-sdk.tar.gz -C /opt \
  && rm -rf /opt/google-cloud-sdk.tar.gz \
  && gcloud config set core/disable_usage_reporting true \
  && gcloud -v

# Firebase tools
RUN npm install -g firebase-tools
