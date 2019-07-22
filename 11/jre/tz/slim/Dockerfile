FROM openjdk:11-jre-slim

RUN apt-get update && apt-get install -y iputils-ping telnet

ENV TZ=America/Sao_Paulo

RUN ln -fs /usr/share/zoneinfo/$TZ /etc/localtime && dpkg-reconfigure -f noninteractive tzdata

ENTRYPOINT date
