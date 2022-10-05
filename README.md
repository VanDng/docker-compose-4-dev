## Compose up

```
docker compose -f "<DockerCompseFilePath>" up -d
```

## Notes

### sqlserver2022 / sqlserver2019

1/ Data directory binding
The container is preconfigured to mount data folders from the container to host.
On the host, prepare folders with the following structure:

```
D:
    DockerVolume
        SqlServer2022 // (or SqlServer2019)
            data
            log
            secrets
```

<br />
2/ Check SQL Server version
Connect to the target server instance and execute the following query.

```
SELECT @@version
```

### smtp4dev

Portal: localhost:3000

https://github.com/rnwood/smtp4dev/wiki/Configuring-Clients
https://github.com/rnwood/smtp4dev/wiki/Configuration

### rabbitmq-3.8

Portal: localhost:15672

https://hub.docker.com/r/bitnami/rabbitmq
