# Docker

## Check running containers
```
$ docker ps
```
## Check container log
```
docker logs -f <container_id>
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

## Run a command
in `bash`
```
$ docker exec -ti <container_name> bash
```
Example:
`docker exec -ti web bash`


## Housekeeping
Delete all images
NOTE: Use at your risk. Should not be used in Production.
```
$ docker rmi $(docker images -a -q)
```
`fish-shell` command:
`docker rmi (docker images -a -q)`


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




