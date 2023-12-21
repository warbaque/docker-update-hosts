# docker-update-hosts

This tool is meant for simple systems without local dns resolver.

Updates `/etc/hosts` automatically when container networks are changed.

Example block
```
# BEGIN DOCKER CONTAINERS
172.17.0.2 container1
172.17.0.3 container2
172.27.0.2 service2
172.27.0.3 service2_db
172.18.0.2 service3
# END DOCKER CONTAINERS
```

## usage

run script as stand-alone updater

```sh
./docker-update-hosts
```

setup script as systemd service
```sh
./setup
```

