# Traefik

[Documentation](https://doc.traefik.io/traefik/)

## Config
`traefik-dynamic.yml` - dynamic config, no need to restart service after making changes

`traefik.yml` - static config that refers to dynamic configs

SSL certificate obtains automatically (email in config should be changed)

## Ports:

- Web - `80`
- Web secure - `443`
- Dashboard - `8080` (not recommended in production)
