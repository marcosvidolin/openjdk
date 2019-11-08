FROM openjdk:11.0.5-jre-slim

ENV TZ=America/Sao_Paulo

RUN apt-get update && apt-get install -y --no-install-recommends iputils-ping telnet \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

RUN ln -fs /usr/share/zoneinfo/$TZ /etc/localtime && dpkg-reconfigure -f noninteractive tzdata