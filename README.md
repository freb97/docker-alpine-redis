# Docker Alpine Redis

Alpine Linux docker image running redis-server and redis-cli with
automatic configuration.

## Getting Started

### Dependencies

* Docker
* Docker-Compose

#### Recommended

* JetBrains IntelliJ
* Visual Studio
* (Visual Studio Code)

### Installation

* Download and dependencies
  * Docker
  * Docker-Compose

### Usage

Start docker container and redis-server instance:

```bash
$ docker-compose up -d
```

Stop docker container

```bash
$ docker-compose stop
```

Connect to docker container via ssh:

```bash
$ sh ./dev-ops/bash.sh
```

Connect to redis-cli:

```bash
$ sh ./dev-ops/cli.sh
```

### Database access

The database file is synced into the ```dumps``` folder
every 10 seconds if 1 or more keys have been updated.

To read or write single database entries use the redis
cli (see Usage).

#### RedisInsight:

For a graphical overview of the database, it is
recommended to use the free RedisInsight software:

- Download RedisInsight from https://redis.com/redis-enterprise/redis-insight/
- Install application and add new database:
  - Host: Docker container IP (find with ```ifconfig en0```)
  - Port: 6379
  - Name: your database name (default "db0")
  - Username: your database username (default none)
  - Name: your database password (default none)
