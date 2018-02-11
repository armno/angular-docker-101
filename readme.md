# angular-docker-101

Learning how to dockerize an Angular app.

0. install docker for mac
1. create an angular app in `client` directory
2. create `dockerfile` in `client` directory
3. update `package.json` -> `npm start` to start dev server with `-H 0.0.0.0`
4. `docker build ...` -> create our own docker image
5. `docker run --rm -p 80:4200 angular-docker/client`
6. create custom nginx docker image
7. create `docker-compose.yml` in root directory
8. `docker-compose up -d --build --remove-orphans`