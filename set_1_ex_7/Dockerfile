FROM ubuntu:16.04
EXPOSE 5000 8000
ENV FRONT_URL http://localhost:5000
ENV API_URL http://localhost:8000
RUN apt update && apt install -y curl git

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash && apt install -y nodejs
RUN git clone https://github.com/docker-hy/backend-example-docker.git
RUN git clone https://github.com/docker-hy/frontend-example-docker.git

WORKDIR /backend-example-docker
RUN touch logs.txt
RUN npm install
WORKDIR /frontend-example-docker
RUN npm install
COPY run.sh run.sh
CMD ./run.sh