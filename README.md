# Commands

Run docker container:

```sh
docker run --rm -it -p 1883:1883 -p 9001:9001 -v ${PWD}/mosquitto.conf:/mosquitto/config/mosquitto.conf -v /mosquitto/data -v /mosquitto/log --name mosquitto eclipse-mosquitto:2.0-openssl
```

Or create named volume and bind to it.

```sh
  --mount source=myvol2,target=/app \
```
