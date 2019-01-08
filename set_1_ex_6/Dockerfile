FROM ubuntu:16.04
EXPOSE 8000
RUN apt update && apt install -y curl git
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker.git
WORKDIR /backend-example-docker
RUN touch logs.txt
RUN npm install
CMD npm start