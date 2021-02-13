# App-Mylar

## First Time Prerequisites

1. `rm ./Data/example/.gitkeep`
2. Run [Traefik](https://github.com/HackingServerHomelab/App-Traefik)

## Running the Containers

1. Update the following lines in [docker-compose.yml](./Docker/docker-compose.yml)
    * `../Data/config:/config`
    * `../Data/comics:/comics`
    * `../Data/downloads:/downloads`
2. Update the Traefik host label in [docker-compose.yml](./Docker/docker-compose.yml)
    * ``"traefik.http.routers.mylar.rule=Host(`localhost`)"``
3. Run `docker-compose -f ./Docker/docker-compose.yml up -d`

## First Time Setup

1. Visit <https://your-ip>
