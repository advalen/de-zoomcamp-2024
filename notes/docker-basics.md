## Docker Basics

Docker is a open-source platform that automates the ***deployment of applications*** stored in a lightweight ***container*** created out of an ***image***. It's a long story, I'll just edit later.

### Basic Docker Commands

1. Run a docker container
```bash
# docker run -it [image name] [params]
docker run -it ubuntu bash
docker run -it --entrypoint=bash python:3.9
```

2. List running containers
```bash
docker ps
```

3. List all docker images
```bash
docker images
```

4. Stop a running container
```bash
# docker stop <CONTAINER_ID>
docker stop e256a64bce77
```

5. Delete a docker container
```bash
# docker rm <CONTAINER_ID>
docker rm 
```

6. Delete a docker image
```bash
# docker rmi <IMAGE_NAME>:<TAG>
docker rmi 

# force delete
docker rmi 
```

### Dockerfile

To reproducibly and seemlessly build a custom docker container, a ***dockerfile*** script is written.

Example:
```dockerfile
FROM python:3.9

RUN  pip install pandas

ENTRYPOINT [ "bash" ]
# The script runs in bash entrypoint rather than in python interactive terminal.
```



Once the dockerfile is finished, it is then used to create the customized python container using ***docker build*** command:

```bash
# docker build [name:tag] [build context]
docker build -t test:pandas .

# build context is the path to the directory of the dockerfile relative to current working directory.
# In this case, the dockerfile is located in the current working directory (.)
```

### Docker Run Applications

docker network create `network-name`

PostgreSQL Server
```bash
docker run -it \
  -e POSTGRES_USER=root \
  -e POSTGRES_PASSWORD=root \
  -e POSTGRES_DB=ny_taxi \
  -v c:/Users/adval/OneDrive/git/data-engineering-zoomcamp-2024/week-1/ny_taxi_postgres_data:/var/lib/postgresql/data:rw \
  -p 5432:5432 \
  --network=pgnetwork \
  --name pgdatabase \
  postgres:13
```

Pgadmin
```bash
docker run -it \
  -e PGADMIN_DEFAULT_EMAIL="admin@admin.com" \
  -e PGADMIN_DEFAULT_PASSWORD="root" \
  -p 8080:80 \
  --network=pgnetwork \
  --name pgadmin \
  dpage/pgadmin4
```