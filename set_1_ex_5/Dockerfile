FROM ubuntu:16.04
EXPOSE 5000
RUN apt update && apt install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN git clone https://github.com/docker-hy/frontend-example-docker.git
WORKDIR /frontend-example-docker
RUN npm install
CMD npm start