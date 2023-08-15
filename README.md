# Docker Manictime Server

install client
https://www.manictime.com/linux/download

run server
https://hub.docker.com/r/manictime/manictimeserver/

```shell
# setup
docker run -v /var/lib/manictimeserver/Data:/app/Data -p 8080:8080 --rm --entrypoint dotnet manictime/manictimeserver Setup.dll -publicurl

# run server
docker run -v /var/lib/manictimeserver/Data:/app/Data -p 8080:8080 manictime/manictimeserver
```

This repository's compose file run server with restart always option.
