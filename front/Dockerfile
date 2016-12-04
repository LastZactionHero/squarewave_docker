FROM nginx

RUN apt-get update -qq && apt-get install -y build-essential curl

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN apt-get install -y nodejs

ADD . /app
WORKDIR /app
RUN npm install