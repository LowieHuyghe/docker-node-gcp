# Docker node-gcp

Docker image with Node for Google Cloud Platform usage

[![Docker Pulls](https://img.shields.io/docker/pulls/lowieh/node-gcp.svg)](https://hub.docker.com/r/lowieh/node-gcp)
[![Docker Stars](https://img.shields.io/docker/stars/lowieh/node-gcp.svg)](https://hub.docker.com/r/lowieh/node-gcp)

Available in versions:
* Node 10.15.0 (tags: `10.15.0`, `10.15`, `10`, `latest`)

Includes:
* Google Cloud SDK @ 229.0.0
* Google Cloud SQL Proxy @ latest
* `get-gae-version`-command which turns any input into a valid Google App Engine version.
  - `get-gae-version v0.0.1  # Gives v0-0-1`

Usage:
```bash
docker pull lowieh/node-gcp:latest
```
