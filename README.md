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

# Importance of docker for data scientists
Improved and seamless container portability: Docker containers run without modification across any desktop, data center, or cloud environment.
Even lighter weight and more granular updates: Multiple processes can be combined within a single container. This makes it possible to build an application that can continue running while one of its parts is taken down for an update or repair.
Automated container creation: Docker can automatically build a container based on application source code.
Container versioning: Docker can track versions of a container image, roll back to previous versions, and trace who built a version and how. It can even upload only the deltas between an existing version and a new one.
Container reuse: Existing containers can be used as base images — essentially like templates for building new containers.
Shared container libraries: Developers can access an open-source registry containing thousands of user-contributed containers.
