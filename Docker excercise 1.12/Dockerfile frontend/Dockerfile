FROM ubuntu:16.04
COPY frontend-example-docker-master /frontend-example-docker-master
WORKDIR /frontend-example-docker-master
CMD ["/bin/bash"]
ENV API_URL=http://localhost:8000/
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install sudo
RUN sudo apt install -y nodejs
RUN npm install
RUN npx browserslist@latest --update-db
CMD ["npm", "start"]
EXPOSE 5000

