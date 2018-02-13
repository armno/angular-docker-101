# angular-docker-101

Learning how to dockerize an Angular app from
[Running Angular applications inside a Docker container - part 1](https://dpopescu.me/2017/03/13/running-angular-applications-inside-a-docker-container-part-1/)

0. install docker for mac
1. create an angular app in `client` directory
2. create `dockerfile` in `client` directory
3. update `package.json` -> `npm start` to start dev server with `-H 0.0.0.0`
4. `docker build ...` -> create our own docker image
5. `docker run --rm -p 80:4200 angular-docker/client`
6. create custom nginx docker image
7. create `docker-compose.yml` in root directory
8. `docker-compose up -d --build --remove-orphans`
9. `docker-compose stop`

## on another machine

1. clone
2. `$ docker-compose up -d --build --remove-orphans`

- `-d` - detatch mode
- `--build` - build images before starting containers
- `--remove-orphans` - remove images that are not defined in the compose file

## get back some spaces

```sh
$ docker image prune -a
```