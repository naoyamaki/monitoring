FROM debian:latest

RUN apt update && apt install -y wget
RUN wget https://github.com/prometheus/node_exporter/releases/download/v1.7.0/node_exporter-1.7.0.linux-amd64.tar.gz
RUN tar -xzvf node_exporter-*.*.tar.gz
WORKDIR /node_exporter-1.7.0.linux-amd64
CMD [ "./node_exporter", "--web.listen-address", "127.0.0.1:9100" ]
