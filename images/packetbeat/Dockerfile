FROM ubuntu:14.04

LABEL version="1.0.0" \
      output="elasticsearch"

RUN apt-get update
RUN apt-get install -y libpcap0.8 curl
RUN curl -L -O https://download.elastic.co/beats/packetbeat/packetbeat_1.2.2_amd64.deb
RUN sudo dpkg -i packetbeat_1.2.2_amd64.deb

COPY ./packetbeat.yml /etc/packetbeat/packetbeat.yml

CMD ["/etc/init.d/packetbeat", "start"]