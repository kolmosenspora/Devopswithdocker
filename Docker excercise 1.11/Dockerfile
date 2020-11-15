FROM ubuntu:16.04
COPY backend-example-docker-master backend-example-docker-master
WORKDIR /backend-example-docker-master
CMD ["/bin/bash"]
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install sudo
RUN sudo apt install -y nodejs
RUN npm install
EXPOSE 8000