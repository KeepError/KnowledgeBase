# Prometheus

[Documentation](https://prometheus.io/docs/introduction/overview/)

## Config

`prometheus.yml`

## Start

```console
$ sudo addgroup nobody
$ sudo usermod -aG nobody nobody
$ sudo chown nobody:nobody config/prometheus.yml
$ docker compose up
```

## Ports:

- Dashboard and metrics - `9090`
