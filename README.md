## Compose up

```
docker compose -f "<DockerCompseFilePath>" up -d
```

## Notes

### sqlserver2022

The container is preconfigured to mount data folders from the container to host.
On the host, prepare folders with the following structure:

```
D:
    DockerVolume
        SqlServer2022
            data
            log
            secrets
```
