# Get image

[official docker image: docker-library/mysql](https://github.com/docker-library/mysql)

[setup instructions](https://github.com/mysql/mysql-docker)

pull the `8.0` image

```
docker pull mysql/mysql-server:8.0
```

# Dockerfile

[tutorial](https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/docker-mysql-getting-started.html)

Instead of local tag, replaced remote tag

tagging mysql 8.0 to remote repo

```
docker tag mysql/mysql-server:8.0 163909562407.dkr.ecr.ca-central-1.amazonaws.com/repository-test:latest
```

push tag to remote repo

```
docker push 163909562407.dkr.ecr.ca-central-1.amazonaws.com/repository-test:latest
```

