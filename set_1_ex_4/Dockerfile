FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl
COPY curler.sh .
RUN chmod +x curler.sh 
CMD ./curler.sh