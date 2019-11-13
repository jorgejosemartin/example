To Run single kafka and single zookeeper 

# Requirements

## Docker

Please export your environment before starting the stack:
```
export DOCKER_HOST_IP=127.0.0.1
```
(that's the default value and you actually don't need to do a thing)

## Docker-Toolbox
If you are using Docker for Mac <= 1.11, or Docker Toolbox for Windows
(your docker machine IP is usually `192.168.99.100`)

Please export your environment before starting the stack:
```
export DOCKER_HOST_IP=192.168.99.100
```

## Single Zookeeper / Single Kafka

This configuration fits most development requirements.

 - Zookeeper will be available at `$DOCKER_HOST_IP:2181`
 - Kafka will be available at `$DOCKER_HOST_IP:9092`


Run with:
```
docker-compose -f zk-single-kafka-single.yml up
docker-compose -f zk-single-kafka-single.yml down
