# Get Docker

https://docs.docker.com/engine/install/ubuntu/



##### permission note

error

```
docker: Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Post http://%2Fvar%2Frun%2Fdocker.sock/v1.24/containers/create: dial unix /var/run/docker.sock: connect: permission denied.
See 'docker run --help'.
```

fix:

```
sudo groupadd docker
sudo usermod -aG docker ${USER}
newgrp docker

su -s ${USER}
docker run hello-world
```


AWS if `Docker-Compose can't connect to Docker Daemon`
```
sudo chown $USER /var/run/docker.sock
```
https://stackoverflow.com/questions/34532696/docker-compose-cant-connect-to-docker-daemon


[stack overflow (worked)](https://stackoverflow.com/questions/48957195/how-to-fix-docker-got-permission-denied-issue)

[digital ocean post](https://www.digitalocean.com/community/questions/how-to-fix-docker-got-permission-denied-while-trying-to-connect-to-the-docker-daemon-socket)



# Test if docker installed properly

[quick start](https://docs.docker.com/get-started/)

run

```
docker run hello-world
```

or

```
docker run -d -p 80:80 docker/getting-started
```

