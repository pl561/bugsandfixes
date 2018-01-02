# Docker general tips

## Installation
[Website](https://docs.docker.com/engine/installation/linux/docker-ce/ubuntu/#install-from-a-package)

### Steps given on the website for Ubuntu 16.04 (check on the website for the security keys)
* sudo apt-get update
* sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common
* curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
* sudo apt-key fingerprint 0EBFCD88
* sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
* sudo apt-get update
* sudo apt-get install docker-ce

## Tests
* sudo docker run hello-world
* sudo docker -it ubuntu bash

## Commands

### Display
* docker ps -l                                to see containers
* docker images                               to see images
* Ctrl+P Ctrl+Q                               to detach from current container
* docker run -it repository_name command      to create a container of an image
* docker commit running_container_id new_name to commit a new docker image from running container id
* docker attach container_id
* docker exec -it container_id bash           to connect a running container with a new session (multiple terminal)
