# Docker

## Check running containers
```
$ docker ps
```

## List images
```
$ docker image ls
```

## Restart
```
$ docker restart <container_name>
```
Example:
`docker restart web`

## Stop
```
$ docker stop <container_name>
```
Example:
`docker stop web`




# Docker Compose
## Build a container using a yaml file
```
$ docker-compose -f <yaml_filename> up --build -d <container>
```
Example:
`docker-compose -f docker-compose-local.yml up --build -d web`

## Stop container in a yaml file
```
$ docker-compose -f <yaml_filename> down
```
Example:
`docker-compose -f docker-compose-local.yml down



