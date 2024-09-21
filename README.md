# trino-dbeaver-docker
How to run `trino` and `dbeaver` locally with `docker compose`

## Start services
```
docker compose up
```

## Open dbeaver UI

http://localhost:8978/

## Setup connection to trino

![trinodb_connect](docs/trinodb_connect.png)

`Host:` `trino`, as the name of the service in the `compose.yaml` file  

```
services:
  trino:
```

`Port:` `8080`, as the container port, the right part of `"8080:8080"` in the `compose.yaml` file  

### Authentication
The default authentication for trino is:

`User name:` `admin`

`User password:` leave it empty

## Learn about Trino
This is a good channel to start learning about Trino

https://www.youtube.com/watch?v=y58sb9bW2mA

Enjoy!

## Stop services
```
docker compose down -v
```
