FROM ubuntu:18.04
RUN mkdir /example
ADD . /example
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_8.x | bash -
RUN apt-get update && apt-get install -y nodejs
RUN cd /example/frontend-example-docker && npm install
EXPOSE 5000
WORKDIR /example/frontend-example-docker
ENTRYPOINT API_URL=http://localhost:8000 npm start

