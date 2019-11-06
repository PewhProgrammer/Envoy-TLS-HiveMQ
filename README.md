# TLS Broker

This is a dockerized application for secure transportation of mqtt data with hivemq ce broker. The tls termination is handled by the envoy proxy application. 

# Install

Docker and Docker Compose has to be installed

# Usage

```console
user@shell:~$ docker-compose up
```

Envoy and Hivemq will be ready.
Hivemq ce might take a while to boot up.

The user can now start publish messages on the port ``8883``. The channel is encrypted by tls. You can test this by using [MQTT Client](https://mqttfx.jensd.de/) with TLS support.


Exit application

```console
user@shell:~$ docker-compose down
```