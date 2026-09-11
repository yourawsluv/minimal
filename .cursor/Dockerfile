FROM ruby:3.2-bookworm

# System packages needed to build native gems (nokogiri, sass-embedded, ffi)
# and to run the Jekyll dev server.
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        build-essential \
        git \
        curl \
        zlib1g-dev \
        libffi-dev \
        libyaml-dev \
    && rm -rf /var/lib/apt/lists/*

RUN gem install bundler
