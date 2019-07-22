FROM openjdk:11-jre-slim

ENV TZ=America/Sao_Paulo

RUN ln -fs /usr/share/zoneinfo/$TZ /etc/localtime && dpkg-reconfigure -f noninteractive tzdata

ENTRYPOINT date
