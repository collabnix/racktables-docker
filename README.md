# Running Racktables inside Docker Container

Follow the below steps to run persistent-Racktables which runs inside Docker containers


# Quickstart

## Clone this Repository

```
git clone https://github.com/collabnix/racktables-docker
cd racktables-docker
```

## Install Docker

```
curl -sSL https://get.docker.com/ | sh
```

## Configuring DNS for your Docker container

Edit daemon.json file

```
 cat /etc/docker/daemon.json
```

```
{
"dns": ["8.8.8.8"]
}
```

## Bring up Racktables Services using Docker Compose

```
docker-compose up
```

## Accessing Racktables UI

Start by browsing to http://localhost/?module=installer&step=5

## Configuration

Look at the env vars available in the `Dockerfile` and `entrypoint.sh`.


