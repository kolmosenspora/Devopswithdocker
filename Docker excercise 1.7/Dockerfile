FROM ubuntu:16.04
WORKDIR /mydir
CMD ["/bin/bash"]
RUN apt-get update && apt-get install -y curl
COPY Dockerscript.sh .
RUN chmod +x Dockerscript.sh
ENTRYPOINT ["sh" , "-c"]

