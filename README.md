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
