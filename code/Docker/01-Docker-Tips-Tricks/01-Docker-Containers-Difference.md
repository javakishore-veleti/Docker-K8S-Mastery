
# Docker "diff" command

Docker "diff" command allow to know the difference between a new Docker image and its new image.

Commands are:

``` sh

docker run --name my-first-image ubuntu:latest touch /MyFirstImageNotes.txt

docker diff my-first-image

docker rm my-first-image

```

![Container Differences](./01-01-containers-diff-command.PNG)

Below is antother output of "docker diff" command. C stands for change and A stands for added.

``` sh

docker run --name my-first-image ubuntu:latest touch /MyFirstImageNotes.txt /bin/MyBinFile.txt

docker diff my-first-image

docker rm my-first-image

```

![Container Differences multiple files](./01-02-containers-diff-cmd-multiple-files.PNG)
