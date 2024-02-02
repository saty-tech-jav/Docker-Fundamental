# NOTES OF DOCKER FUNDAMENTALS FOR CREATING IMAGES

## PROBLEM STATEMENT IF WE ARE NOT USING DOCKER  statement-1

1.Time consuming <br> 
2.Compatibility issues <br>
3.Error prone issues<br>

  Developer will devlope java code having version of java 10 and when 
  QA will run this code on his system having java version 8 it will not
  work .Hence docker came into picture

  ## SOLUTION WITH DOCKER

  1.Docker packages the application and dependency required to run the application into the
    single bundle and ship it to the target environment.In docker world we call this bundle with
    as image.

  2.When we run this image in QA environment this creates an isolated environment for the application
    to run by installing all packages/dependency we call this isolated environment as container.


  ## PROBLEM STATEMENT IF WE ARE NOT USING DOCKER  Problem statement-2

  1.If we are having three application running on same host for security reason we need to
       isolated the application .Solution comes in our mind to deploy these three application
       on three different host but this will not work as it is more cost effective

  2.Second thought will three different VMs on single host.This is also effective but
      VM takes lost of resources.

  ## SOLUTION AFTER IMPLEMENTING DOCKER

  1. We will create three 3 images of 3 application and will run this application by this way
       they will run in isolated environment which is called Containers.

    *******IMPORTNAT DEFINATION*******

  >Docker is an open platform for developing, shipping, and running applications. 
  >We can create any number of container using same image.
  >Docker images are sharable through container registry like docker hub ,AWS ECR.


  ## DOCKER ARCHITECTURE

1. Docker uses a client-server architecture.

  2.The Docker client talks to the Docker daemon, which does the heavy lifting 
    of building, running, and distributing your Docker containers.

  3.The Docker client and daemon communicate using a REST API, over UNIX 
    sockets or a network interface.

  ### DOCKER DAEMON 

  1.The Docker daemon (dockerd) listens for Docker API requests and manages Docker objects such as 
  images, containers, networks, and volumes. 

  ### DOCKER client

  1.The Docker client (docker) is the primary way that many Docker users interact with Docker. When you use commands such as docker run,
   the client sends these commands to dockerd, which carries them out.

  ### DOCKER DESKTOP

  1.Docker Desktop is an easy-to-install application for your Mac, Windows or Linux environment that enables you to 
  build and share containerized applications and microservices.

  ### DOCKER REGISTRY

  1.A Docker registry stores Docker images

  ### DOCKER OBJECTS 

  1.When you use Docker, you are creating and using 
    images, containers, networks, volumes, plugins, and other objects.

  ### DOCKER IMAGES 

  1.An image is a read-only template with instructions for creating a Docker container.

  ### DOCKER CONTAINERS 

  1.A container is a runnable instance of an image







