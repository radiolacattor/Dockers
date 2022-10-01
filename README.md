# Docker-compose for Simple SpringBoot Based App

### Put `docker-compose.yml` to the root of the repository

#### Put `Dockerfile` from the `Dockerfile_for_node/` to the `node-app/` directory
#### Put `Dockerfile` from the `Dockerfile_for_maven/` to the `spring-boot-app/` directory

#### Define variables 
`POSTGRES_USER`  `POSTGRES_PASSWORD` `POSTGRES_DB` in `docker-compose.yml`

#### Run:

```
docker-compose up --build -d
```