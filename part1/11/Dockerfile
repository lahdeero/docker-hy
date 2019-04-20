FROM ubuntu:18.04
RUN mkdir /example
ADD . /example
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt-get update && apt-get install -y nodejs
EXPOSE 8000
WORKDIR /example/backend-example-docker
RUN npm install
ENTRYPOINT FRONT_URL=http://localhost:5000 npm start

