# Docker ELK Stack

Docker powered ELK stack extended by PacketBeat and TopBeat

### Installation

Run docker-compose

```sh
docker-compose up -d
```

Load Beats dashboard (change elasticsearch container identifier)

```sh
.load_beats_dashboard.sh elk_elasticsearch_1
```

### Kibana

Browse to `your-docker-instance-ip:5601`, e.g. `192.168.99.100:5601`

If you are using docker-machine on a Mac, simply run

```sh
open http:`docker-machine ip`:5601
```

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/21stio/docker-elk-stack/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

