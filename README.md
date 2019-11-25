# Simple http 'hello world' for Docker workshop
> Based on the work by [adam-golab/docker-hello-world](https://github.com/adam-golab/docker-hello-world)

[![Docker Pulls](https://img.shields.io/docker/pulls/stefanvangastel/hello-world.svg)](https://hub.docker.com/r/stefanvangastel/hello-world/)

This image is a simple 'Hello World' in an HTTP server to be used in a Docker workshop. When receive an request (GET /) this image will return the `Hello World`.

It shows `Hello <WORLD>` for every request, so it is possible to customize the response.

## Running a simple test
    docker run --rm -it -p 8000:8000 stefanvangastel/hello-world

Will result in a single instance running on the provided PORT or 8000 by default.

## Configuration

|Environment Variable|Default|Description|
|:-----:|:-----:|:----------|
|PORT|8000|Set the Listen Port to access the hello-world container.|
|WORLD|World|Set the string that will be concatenated to Hello in the response.|
