# Docker
----------
- Package software into unit for development, Shipment, deployment.
- Shipment ------> Fortend Component + Backend Workers + DB + Env/Libs/Dependencies

# Image
---------
- Executable package of software lightweight and standalone.

# Container
------------
- When images run on docker engine, they will referred as containers.
- Multiple containers run on the same machine.

# Docker Engine
-----------------
- Which is used run your docker containers.

# Docker hub
-------------
1. Sign Up
2. Docker Login
   User ID 
   Password
   
Docker Commands:
----------------

# Docker Commands
---------------
1) docker --version
2) docker images ---> list of images available
3) docker run <image_name>:<tag>    ---> create a container based on the given image, 
     with a random name for the container
     docker run -d --name <custom name>  <image name>   ---->  create a container based on the given image, with a name provided
4) docker run -d <image_name>:<tag>  ---> run the container as a process
5) docker stop <container name>
6) dokcer pull <image name>:<tag>  
        - tag is optional
        - if tag is not provided it will download the latest image
7) docker start <container name>  or <container id>
8) docker ps -a ---> list of container running
9) docker rm <container name>   -> to remove a conatiner
10)docker logs <conatiner name>
