#### Useful utilities
***
- This project holds some useful utilities like `docker compose`  for brokers & databases, bash scripts for simple manual tasks. 



#### Docker Compose
***
-  The [docker compose](./docker/docker-compose.yml) holds multiple pre-configured services. The list of services present in that file are : 

| Service Name | Port       | Service type                    | Depedencies |
|--------------|------------|---------------------------------|-------------|
| zookeeper    | 2181       | Co-ordination service for Kafka | N/A         |
| kafka        | 19092/9092 | broker                          | zookeeper   |
| kafka-ui     | 8080       | UI for Kafka                    | kafka       |
| mysql        | 3306       | database                        | N/A         |
| postgresql   | 5432       | database                        | N/A         |
