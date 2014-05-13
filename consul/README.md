# Docker container of consul.io

## Install this docker image

```
docker pull domabo/consul
```

## Run image

```
docker run -i -t --rm -n -p 8500:8500 domabo/consul /bin/bash
```

## Bootstrap consul

```
consul agent -bootstrap -server -client=0.0.0.0 -data-dir /tmp/ -ui-dir /usr/local/consul-web-ui
```

Note: for testing purposes only, exposes HTTP API and UI on all host ports

## Look at web ui

```
curl [serverip]:8500/ui/
```
