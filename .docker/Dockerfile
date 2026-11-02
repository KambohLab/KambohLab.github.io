# start with official ruby docker image as base
FROM ruby:3.3-bundler

# set working directory within container
WORKDIR /usr/src/app

# pull in ruby (jekyll) and python (cite process) package info
COPY Gemfile Gemfile.lock _cite/requirements.txt ./

# install ruby packages
RUN VERSION=$(grep -A 1 'BUNDLED WITH' Gemfile.lock | tail -n 1 | xargs); \
    gem install bundler --version ${VERSION} && \
    bundle _${VERSION}_ install

# Use the official Python image with your desired version
FROM python:3.12-slim

# Set the working directory
WORKDIR /workspace

# Install system dependencies if your requirements need compilation tools
RUN apt-get update && apt-get install -y --no-install-recommends \
    build-essential \
    && rm -rf /var/lib/apt/lists/*

# Copy and install python packages
COPY requirements.txt .
RUN pip install --no-cache-dir --upgrade --requirement requirements.txt

# Install watchdog
RUN pip install "watchdog[watchmedo]==3.0.0"

# ports used by jekyll
EXPOSE 4000
EXPOSE 35729

# run jekyll and cite process
COPY .docker/entrypoint.sh /var
CMD [ "/var/entrypoint.sh" ]
