# Docker-learnings

The basic idea behind docker is to make mulitple systems compactible for a particlular task. The same can be achieved by:-
1. Making an environment that is similar to the initial computer in which the program/ software is developed.
2. Making a virtual Machine.

The advantage of using docker is that it is light weight and provides similar functionality as virtual machines.

## Let's look at a comparison with Virtual Machine and docker
<div align="center"><img src="https://github.com/nelson123-lab/Dockor-learnings/blob/2827146ed6e21e072232a7ae2aacf34c7817e84b/VM_vs_Docker.png" width="900"/></div>


Docker is tool which is used to automate the deployment of applications in light weight containers so that many applications can work efficiently in different environments.

! dockerignore and gitignore are for ignoring the local dependency of the working hardware.
## Docker Essential Components:-

Docker File 
- like a blueprint for building docker images.
Docker Image
- Template for running docker containers.
Containers
- Run in progress.
Volume
- Dedicated folder on the host machine.
Docker compose 
- To run multiple docker containers at the same time.

## Docker Commands
docker ps -- list all the running containers in your system.
docker build -t tagname/demoapp:1.0 -- to make a docker image.
docker run id -- running a container
docker run -p 5000:8080  -- port forwarding.
docker volume create name -- to create a volume
