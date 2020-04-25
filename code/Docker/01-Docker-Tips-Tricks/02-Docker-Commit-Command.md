
# 01  Docker commands that users the  "commit" command

``` sh

docker run --name container-with-git ubuntu:latest /bin/bash -c "apt-get update -y ; apt-get upgrade -y ;  apt-get install git -y "

docker commit -a "your_user_name_here" -m "Installed git" container-with-git image-ubuntu-with-git


```

![docker run with git install](./02-01-containers-with-git-install.PNG)

![docker commit of an existing container](./02-02-containerswith-git-commit.PNG)
