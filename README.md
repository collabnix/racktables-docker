# Running Racktables inside Docker Container

This repository is an extension of work from original [ptman/racktables-docker](https://github.com/ptman/racktables-docker). This repository adds the below functionalities:

- Persistent Racktables Database

- Report Generation

![My Image](https://github.com/collabnix/racktables-docker/blob/master/racktables1.png)

![My Image](https://github.com/collabnix/racktables-docker/blob/master/racktables2.png)


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

## Install Docker Compose

```
curl -L https://github.com/docker/compose/releases/download/1.23.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```

## Configuring DNS for your Docker container(in case you're behind the firewall)

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
docker-compose build
docker-compose up -d 
```

## Accessing Racktables UI

Start by browsing to http://localhost/?module=installer&step=5

# Contributor

[Ajeet S Raina](ajeetraina@gmail.com)


