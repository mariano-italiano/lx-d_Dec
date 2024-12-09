FROM ubuntu:22.04
RUN apt-get update
RUN apt-get install curl postfix -y

MAINTAINER Marcin Kujawski

WORKDIR /app

ENTRYPOINT ["tail"]

CMD ["-f", "/dev/null"]
