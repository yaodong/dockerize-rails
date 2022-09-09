FROM ruby:3.1.2-slim-bullseye AS builder

WORKDIR /app

ARG RAILS_ENV="production"
ARG NODE_ENV="production"

ENV RAILS_ENV=${RAILS_ENV} \
    NODE_ENV=${NODE_ENV}

RUN apt-get update -qq && \
    apt-get install -y --no-install-recommends build-essential curl git libpq-dev
