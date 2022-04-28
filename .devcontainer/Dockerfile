# Base image setup
ARG PYTHON_VERSION=3.10.4-buster
FROM python:${PYTHON_VERSION}
ENV PYTHONUNBUFFERED=1

# Debian updates
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive && apt-get -y install --no-install-recommends sudo && sudo apt -y update

# Install node LTS (due to uWebSockets.js build limitations)
RUN curl -fsSL https://deb.nodesource.com/setup_lts.x | bash - && apt-get install -y nodejs