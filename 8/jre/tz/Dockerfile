FROM openjdk:8-jre

ENV TZ=America/Sao_Paulo

RUN apt-get update && apt-get install -y --no-install-recommends \
  telnet \
  && apt-get clean \
  && rm -rf /var/lib/apt/lists/*

RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
