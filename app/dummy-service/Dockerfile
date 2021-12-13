FROM ruby:2.4

RUN mkdir /app
ADD Gemfile /app/Gemfile
COPY . /app
WORKDIR /app
RUN bundle install


EXPOSE 5000
CMD ["bundle", "exec", "foreman", "start"]
