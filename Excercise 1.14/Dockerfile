FROM ruby:2.6.0
COPY rails-example-project-master rails-example-project-master
CMD ["/bin/bash"]
WORKDIR /rails-example-project-master
ENV RAILS_ENV=development
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install sudo
RUN sudo apt install -y nodejs
RUN gem install bundler
RUN gem install rails
RUN bundle install
RUN bin/rails db:migrate
WORKDIR /rails-example-project-master
CMD ["rails", "s"]
EXPOSE 3000
