# racktables-docker

[![](https://img.shields.io/docker/pulls/ptman/racktables.svg)](https://hub.docker.com/r/ptman/racktables/)
[![](https://img.shields.io/docker/automated/ptman/racktables.svg)](https://hub.docker.com/r/ptman/racktables/builds/)
[![](https://images.microbadger.com/badges/image/ptman/racktables.svg)](http://microbadger.com/images/ptman/racktables)

## Quickstart

Note that this isn't a production setup, but fairly close. Make sure to change
the configuration if you intend to use it in production.

    docker-compose up
    # Start by browsing to http://localhost/?module=installer&step=5

## Configuration

Look at the env vars available in the `Dockerfile` and `entrypoint.sh`.

## Troubleshooting

In case you encounter issue related to APK and error message(being behind the corporate firewall) stating that timed-out issue, you might need to add DNS for your containers

```
 cat /etc/docker/daemon.json
```

```
{
"dns": ["8.8.8.8", "10.8.8.8" ]
}
```
