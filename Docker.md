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
    
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

MobileService
--------------
1. OpenJdk11-jdk
2. Mongo
3. MobileService Jar file

To create docker image
----------------------

Step 1: To create a jar file
-----------------------------
1. Use Terminal/cmd ------------> maven install -DSkipTests
2. Use Maven tool in ItelliJ IDE
3. Run the jar file ------------> java -jar demo-0.0.1-SNAPSHOT.jar

Step 2: To Create a Docker File
--------------------------------
1. Create a docker file inside a project root directory.
2. We need base image of our application
   OpenJDK -----------------> Docker
   
Step 3: Build image based on docker file
-----------------------------------------
1. sudo docker build -t rajeev1583/oneplusservice:v1 .
2. sudo docker run -p 9091:8082 --name oneplusservice_container rajeev1583/oneplusservice:v1

Step 4: After building your image push into a docker hub
- docker login
  username
  password
  
-  sudo docker push rajeev1583/oneplusservice:v1

-------------------------------------------------------------------------------------------------------------------------------------

Assignment
-----------
Create a ProductService 
-----------------------
Model -----> Product.java
Repository ----> ProductRepository.java
Service ------> ProductService.java
        ------> ProductServiceImpl.java
        
Controller ------> ProductController.java 

Create a docker file, Build image and push the image into Dcoker Hub.
  
  
  
  

    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
