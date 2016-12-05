FROM nginx


RUN apt-get update -qq && apt-get install -y build-essential curl

RUN curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb http://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -

RUN apt-get update -qq
RUN apt-get install -y nodejs yarn

ADD ./src /app
WORKDIR /app
RUN yarn install
