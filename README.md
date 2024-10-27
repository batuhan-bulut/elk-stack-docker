# ELK Stack with Docker Swarm
On this repository, you can install ELK Stack (*Elasticsearch*, *Logstash*, *Kibana*) with one command.

You can follow the guide in here [Medium Link](https://bulutbatuhan.medium.com/3a9b7123486c "Medium Link") or follow the guide below.

## Installation
- Download the repo on your local.
- Run `docker compose up -d` on the same directory.
- Get Kibana Configure URL
 - `docker compose logs kibana | grep 'get started'`
- Get Enrollment Token from Elasticsearch
 - `docker exec -u elasticsearch elasticsearch-container bin/elasticsearch-create-enrollment-token --scope kibana`
- Paste the Enrollment token to Kibana and complete installation.

Login Kibana from http://localhost:5601
- Default Credentials:
 - Username: *elastic*
 - Password: *rockyou*
