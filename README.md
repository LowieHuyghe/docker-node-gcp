# Docker node-gcp

Docker image with Node for Google Cloud Platform usage

[![CircleCI](https://circleci.com/gh/LowieHuyghe/docker-node-gcp.svg?style=svg)](https://circleci.com/gh/LowieHuyghe/docker-node-gcp)
[![Docker Pulls](https://img.shields.io/docker/pulls/lowieh/node-gcp.svg)](https://hub.docker.com/r/lowieh/node-gcp)
[![Docker Stars](https://img.shields.io/docker/stars/lowieh/node-gcp.svg)](https://hub.docker.com/r/lowieh/node-gcp)

Available in versions:
* Node 8.15.0 (tags: `8.15.0`, `8.15`, `8`)
* Node 10.15.0 (tags: `10.15.0`, `10.15`, `10`, `latest`)

Includes:
* Google Cloud SDK @ 206.0.0
* `get-gae-version`-command which turns any input into a valid Google App Engine version.
  - `get-gae-version v0.0.1  # Gives v0-0-1`

Usage:
```bash
docker pull lowieh/node-gcp:latest
```
