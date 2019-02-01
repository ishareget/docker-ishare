# Docker iShare

Run iShare project in Docker.

## Setup

1. Clone this project
2. chmod 777 for .docker/mariadb/data

## Usage

1. Download dependence project using `git submodule` command.
2. Use `docker-compose` to run whole project.


## Update 

```bash
git submodule update --init --remote
```

or

```bash
git submodule foreach --recursive git pull origin master
```

## Run
```bash
docker-compose up -d
```

or rebuild and run

```
docker-compose up -d --build
```

## Danger

Force to rebuild

```sh
 docker-compose rm --all &&
 docker-compose pull &&
 docker-compose build --no-cache &&
 docker-compose up -d --force-recreate
```

