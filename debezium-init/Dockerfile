FROM alpine:latest
RUN apk update
RUN apk add curl
COPY param.json /tmp
CMD curl -i -v -X POST -H "Accept:application/json" -H "Content-Type:application/json" -d @/tmp/param.json debezium:8083/connectors/
