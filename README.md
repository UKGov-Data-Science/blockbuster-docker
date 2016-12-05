# blockbuster-docker

The [Dockerfile](Dockerfile) in this repository fixes an environment for developing the [blockbuster](https://github.com/mammykins/blockbuster/) package to ensure reproducibility going forward, and to make package development cross platform easier.

## How to use

A [Dockerfile](Dockerfile) provides a list of instructions for building a lightweight virtual machine (contaienr) in which a process can be run.

There are two ways to make use of this container image:

* Clone the contents of this repo, and recreate the docker container locally using `docker build -t blockbuster:latest .`.
* Pull the complete container from the automatic build that takes place on [docker hub](https://hub.docker.com/r/ukgovdatascience/blockbuster/) with `docker pull ukgovdatascience/latest`

For each of these methods, you will need to have docker installed.
A good guide for installing docker is provided [here](https://docs.docker.com/engine/getstarted/step_one/).

The container can then be run using `docker run -it ukgovdatascience/blockbuster:latest /bin/bash` to open a shell within the container.
