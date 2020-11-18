FROM ubuntu:16.04
COPY backend-example-docker-master backend-example-docker-master
CMD ["/bin/bash"]
ENV FRONT_URL=http://localhost:5000
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install sudo
RUN sudo apt install -y nodejs
WORKDIR /backend-example-docker-master
RUN npm install
CMD ["npm", "start"]
EXPOSE 8000
