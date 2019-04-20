FROM ruby:2.6.0
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get update && apt-get install -y nodejs
CMD mkdir /usr/src/app
COPY ./rails-example-project /usr/src/app
WORKDIR /usr/src/app
RUN bundle install
RUN rails db:migrate 
ENTRYPOINT rails s
