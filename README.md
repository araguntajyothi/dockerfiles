### Docker files

Docker file is a declarative way of creating our own images. Docker will give us some syntax to create our own image.

First Instruction is FROM

Filename should be Dockerfile

### how to build image from Dockerfile

```
docker build -t [docker-hub-URL]/[your-username]/[image-name]:version .
```

### how to psuh image to dockerhub

```
docker push [docker-hub-URL]/[your-username]/[image-name]:version
```