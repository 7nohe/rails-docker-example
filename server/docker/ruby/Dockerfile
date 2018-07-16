FROM ruby:2.5
RUN apt-get update -qq && apt-get install -y build-essential libpq-dev nodejs
ARG  APP_NAME
RUN echo "$APP_NAME"
RUN mkdir "/$APP_NAME"
WORKDIR "/$APP_NAME"
COPY Gemfile "/$APP_NAME/Gemfile"
COPY Gemfile.lock "/$APP_NAME/Gemfile.lock"
RUN bundle install
COPY . "/$APP_NAME"