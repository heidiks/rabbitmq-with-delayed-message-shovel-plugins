RabbitMQ with management and compatible version of the delayed message exchange and shovel plugins

## Versions
- [latest](https://github.com/heidiks/rabbitmq-with-delayed-message-shovel-plugins/blob/master/versions/latest/Dockerfile)
- [3.8.7](https://github.com/heidiks/rabbitmq-with-delayed-message-shovel-plugins/blob/master/versions/3.8.7/Dockerfile)

## Running
#### Image

    docker run heidiks/rabbitmq-with-delayed-message-shovel-plugins:latest


#### Docker compose sample:
```YAML
version: '3.3'

services:
  rabbit:
    image: heidiks/rabbitmq-with-delayed-message-shovel-plugins:latest
    environment:
      - RABBITMQ_DEFAULT_USER=admin
      - RABBITMQ_DEFAULT_PASS=password
    ports:
      - "5672:5672"
      - "15672:15672"
```

## Environment
The environment variables are the same as the [official image](https://hub.docker.com/_/rabbitmq/)
- Sample
    - RABBITMQ_DEFAULT_USER=admin
    - RABBITMQ_DEFAULT_PASS=password


