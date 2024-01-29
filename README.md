# dockers

Dockers is designed to create sandbox environment for web projects

## project overview

Docker images can be built under following directories, `mariadb`, `nginx`, `php-fpm`. For instance, nginx image can be built with following docker cmd.

```bash
> cd ~/dockers/nginx
> docker build .
```

Below are directories that host `Dockerfile` to build docker images:

```bash
── dockers
   ├── jenkins
   ├── k6
   ├── mariadb
   ├── nginx
   └── php-fpm
```

`dockers-demo/docker-compose.yml` (along with `dockers/.env`) is to compose docker containers built from.

### Building(Re-building) all docker images using `docker-compose`

```bash
> cd ~/dockers
> docker-compose build
```

### Start/Stop docker containers using `docker-compose`

```bash
> cd ~/dockers
> docker-compose up -d
```

```bash
> cd ~/dockers
> docker-compose down
```
