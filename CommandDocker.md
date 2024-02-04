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

1.docker build -t sat/first-image:latest .
  (sat is name of repo on docker hub and first image is tag)

### RUN IMAGES==CONTAINER

1.docker run sat/first-image

![image will also be present in desktop](allimage/image10.png)

### PUSH IMAGE TO DOCKER HUB

