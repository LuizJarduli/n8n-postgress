# n8n with PostgreSQL

Starts n8n with PostgreSQL as database. This example was taken from [`this n8n repo`](https://github.com/n8n-io/n8n/blob/master/docker/compose/withPostgres/init-data.sh)

## Start

First copy the contents of .env.example to a file .env with the command in the repository root:

```sh
cp ./.env.example /.env
```

To start n8n with PostgreSQL simply start docker-compose by executing the following
command in the current folder.

**IMPORTANT:** But before you do that change the default users and passwords in the [`.env`](.env) file!

```sh
docker-compose up -d

# Docker compose v2 +
docker compose up -d
```

To stop it execute:

```sh
docker-compose stop

# Docker compose v2 +
docker compose stop
```

## Configuration

The default name of the database, user and password for PostgreSQL can be changed in the [`.env`](.env) file in the current directory.
