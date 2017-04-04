FROM debian:7
MAINTAINER Alteom <contact@alteom.com>

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y openjdk-6-jdk python wget unzip

RUN wget https://downloads.typesafe.com/play/1.2.5.6/play-1.2.5.6.zip
RUN unzip play-1.2.5.6.zip -d / && rm play-1.2.5.6.zip && chmod a+x /play-1.2.5.6/play
ENV PATH $PATH:/play-1.2.5.6

EXPOSE 9000
RUN mkdir /app
RUN mv /play-1.2.5.6/modules / && ln -s /modules /play-1.2.5.6/modules
WORKDIR /app

CMD ["play", "run"]