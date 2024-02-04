# IMPORTNAT COMMAND FOR DOCKER

## CONNECTING TO DOCKER HUB

## If not able to login on docker

<br>
$ winpty docker login $ACR_REGISTRY
<br>
Username: appacr
<br>
Password:
<br>
Login Succeeded
<br>

normal way:docker login -u LOGIN -p PASSWORD

## DOCKER BASIC COMMAND

### BUILD IMAGES

1.docker build -t satytechjava/first-image:latest .
  (satytechjava is the user name of dockerhub and first-image is tag)

### RUN IMAGES==CONTAINER

1.docker run sat/first-image

![image will also be present in desktop](allimage/image10.png)

### RUN IMAGE IN BACKGROUND PROBLEM SOLVED GOING TO ANOTHER TERMINAL

1.docker run -d nginx   (-d is called detached mode)


### PUSH IMAGE TO DOCKER HUB

1.docker push satytechjava/my-image

### PULL IMAGE FROM DOCKER HUB

1.docker pull satytech/my-image

### DOCKER IMAGES LIST

1.docker images

### LIST OF RUNNING CONTAINER

1.docker ps

### LIST OF ALL CONTAINER RUNNING AND STOPPED

1.docker ps -a

### START A CONTAINER

1. docker start containerid

### STOP A CONTAINER

1.docker stop containerid

### PORT MAPPING IN DOCKER

1.By mapping ports between the host machine and containers, we establish a bridge for data          exchange. 
<br>

2.docker run -p <HostPort:containerport> imagename:tag 
<br>

3.docker run -p 80:80 -d nginx

<br>

4.curl http://localhost:80

<br>

### REMOVE A STOP CONTAINER

1.Running container cannot be removed so first stopped it 
  1.1 docker stop e7f1e36b1365 15c2c2bc0525
  1.2 docker rm e7f1e36b1365 15c2c2bc0525
  1.3 then for checking docker ps -a

### GIVING NAME TO CONTAINER

1.docker run --name test -d nginx

### RENAME A CONTAINER

1.docker rename test test1(new name)

### DELETE A IMAGE

1.Image will be deleted when container will be in stop state

2.docker rmi nginx

### HELP COMMAND

1.docker run --help

