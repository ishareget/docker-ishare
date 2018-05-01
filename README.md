# Docker iShare

Run iShare project in Docker.

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