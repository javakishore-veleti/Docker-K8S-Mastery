
# 01  Docker commands that uses the  "commit" command

## docker run command installing git in a container

``` sh

docker run --name container-with-git ubuntu:latest /bin/bash -c \
    "apt-get update -y ; apt-get upgrade -y ;  apt-get install git -y "

```

![docker run with git install](./images/02-01-containers-with-git-install.PNG)

## docker commit command

Docker command that commits an existing image. Ensure to give appropriate name by replacing the text "your_user_name_here" below

``` sh
docker commit -a "your_user_name_here" -m "Installed git" container-with-git image-ubuntu-with-git
```

![docker commit of an existing container](./images/02-02-containerswith-git-commit.PNG)

## docker commit(ed) image further usage

Below commands show how we can usage the above committed image to create future containers.

``` sh
docker run --name git-container --entrypoint git  image-ubuntu-with-git  

```

![docker container output from commited image](./images/02-03-container-git-output.PNG)