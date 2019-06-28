# oh-my-docker-container

Oh My Docker Container! My first venture into the world of docker containers by containerising a Python App.
You can get started with Docker here: https://docs.docker.com/

## Dockerfile
Contains settings such as base image for the container and Python version, as well as dependencies on build to produce the container image.

## Building the Image

To tag the image `hello-world-python` and build it, from the root directory in the terminal:

```bash

docker build --tag hello-world-python .

```

## Run the image as a container

Here, the container name is: `hello-world-python-container`

To start the application as a container:

```bash

docker run --name hello-world-python-container -p 5000:5000 hello-world-python

```

## Other useful Docker CLI commands

To display a list of running containers:

`docker ps`

To stop running one or more running containers:

`docker container stop hello-world-python-container`

To remove one or more containers:

`docker container rm hello-world-python-container`

Confirm the container is no longer running:

`docker ps`