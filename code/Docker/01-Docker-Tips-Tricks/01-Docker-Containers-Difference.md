
# Docker "diff" command

Docker "diff" command allow to know the difference between a new Docker image and its new image.

Commands are:

``` sh

docker run --name my-first-image ubuntu:latest touch /MyFirstImageNotes.txt

docker diff my-first-image

```

![Container Differences](./01-docker-containers-diff-command.png)


