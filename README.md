# Keycloak

This brings up a containerized environment running Keycloak 18.0.1 with a Postgres backend, and [Traefik][] as a front-end https proxy.

[traefik]: https://traefik.io

## Configuration

Rename `example.env` to `.env` and edit `.env` as you see fit.

Whatever value you use for `KEYCLOAK_HOSTNAME` must be a resolvable name. For example, if you want to access Keycloak as `keycloak.local`, you might need to add an alias for `localhost` in your `/etc/hosts` file:

```
127.0.0.1 localhost localhost.localdomain localhost4 localhost4.localdomain4 keycloak.local
```

## Starting

To bring up the containers and watch their logs on the console:

```
docker-compose up
```

To bring up the containers in the background:

```
docker-compose up -d
```
