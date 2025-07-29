# portainer-ce

## Run it docker-compose 

```shell
> git@github.com/luislopescmc/portainer-ce.git
> cd portainer-ce
> docker-compose up -d
```

## docker run
```
$ docker volume create portainer_data
$ docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always \
 -v /var/run/docker.sock:/var/run/docker.sock \
 -v portainer_data:/data portainer/portainer-ce:lts
```


 https://docs.portainer.io/start/install-ce/server/docker/linux
 https://earthly.dev/blog/portainer-for-docker-container-management
