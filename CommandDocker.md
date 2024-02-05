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

### 1.BUILD IMAGES

1.docker build -t satytechjava/first-image:latest .
  (satytechjava is the user name of dockerhub and first-image is tag)

### 2.RUN IMAGES==CONTAINER

1.docker run sat/first-image

![image will also be present in desktop](allimage/image10.png)

### 3.RUN IMAGE IN BACKGROUND PROBLEM SOLVED GOING TO ANOTHER TERMINAL

1.docker run -d nginx   (-d is called detached mode)


### 4.PUSH IMAGE TO DOCKER HUB

1.docker push satytechjava/my-image

### 5.PULL IMAGE FROM DOCKER HUB

1.docker pull satytech/my-image

### 6.DOCKER IMAGES LIST

1.docker images

### 7.LIST OF RUNNING CONTAINER

1.docker ps

### 8.LIST OF ALL CONTAINER RUNNING AND STOPPED

1.docker ps -a

### 9.START A CONTAINER

1. docker start containerid

### 10.STOP A CONTAINER

1.docker stop containerid

### 11.PORT MAPPING IN DOCKER

1.By mapping ports between the host machine and containers, we establish a bridge for data          exchange. 
<br>

2.docker run -p <HostPort:containerport> imagename:tag 
<br>

3.docker run -p 80:80 -d nginx

<br>

4.curl http://localhost:80

<br>

### 12.REMOVE A STOP CONTAINER

1.Running container cannot be removed so first stopped it 
<br>
  1.1 docker stop e7f1e36b1365 15c2c2bc0525
<br>
  1.2 docker rm e7f1e36b1365 15c2c2bc0525
<br>
  1.3 then for checking docker ps -a
<br>

### 13.GIVING NAME TO CONTAINER

1.docker run --name test -d nginx

### 14.RENAME A CONTAINER

1.docker rename test test1(new name)

### 15.DELETE A IMAGE

1.Image will be deleted when container will be in stop state

2.docker rmi nginx

### 16.HELP COMMAND

1.docker run --help

