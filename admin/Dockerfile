FROM ruby:3.1.3

RUN apt-get update && apt-get install -y \
    build-essential \
    libpq-dev \
    npm \
    node.js \
    postgresql-client \
    yarn
WORKDIR /loto-searcher/admin
COPY Gemfile Gemfile.lock /loto-searcher/admin/
RUN bundle install