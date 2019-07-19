FROM openjdk:8-jre-alpine

RUN apk update \
        && apk add tzdata \
        && apk add busybox-extras

RUN cp /usr/share/zoneinfo/America/Sao_Paulo /etc/localtime
RUN echo "America/Sao_Paulo" > /etc/timezone
RUN date
RUN apk del tzdata

ENTRYPOINT date
