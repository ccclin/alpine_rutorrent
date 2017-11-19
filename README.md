# Alpine Rutorrent
Docker Image for rutorrent/rtorrent wiht ARM

Base on
 - [linuxserver/docker-rutorrent](https://github.com/linuxserver/docker-rutorrent)
 - [linuxserver/docker-baseimage-alpine](https://github.com/linuxserver/docker-baseimage-alpine)

## Build Base OS Docker Image
```
docker build -t <YOUR_Dockerfile_base> -f ./Dockerfile_base .
```

## Build rutorrent Docker Image
```
docker build -t <YOUR_Dockerfile_rutorrent> -f ./Dockerfile_base .
```

## Run with Docker Compose Yaml File
Edit your confing on `docker-compose.yml`

start
```
docker-compose -f ./docker-compose.yml up -d
```

stop
```
docker-compose -f ./docker-compose.yml down
```
