FROM ruby:2.6

WORKDIR /app

COPY . ./

RUN apt-get update && apt-get install -y curl
RUN bundle install
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs


RUN rails db:migrate
CMD ["rails", "s"]

# I changed ruby version -> 2.6.3 in Gemfile
