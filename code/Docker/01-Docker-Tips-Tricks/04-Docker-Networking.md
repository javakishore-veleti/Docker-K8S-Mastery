# Docket networking commands and attributes

## Docker container with no outbound access

Below creates a Python container with "--net none", which removes outbound network to the container.

``` sh

docker run --rm --name python-container-with-no-net --net none python:3.7 ip addr

```

![container with no outbout network](./images/04-01-container-with-no-outbount-net.PNG)