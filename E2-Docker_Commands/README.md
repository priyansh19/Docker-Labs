# Docker Commands

As of now we are done with installation part of docker-ce. If you haven't done it till now then go to the [README.md](https://github.com/priyansh19/Fun-With-Docker/blob/master/README.md) 

Now let's start learning Basic docker Commands with thier hands-on ..
```shell
 _                    _ _               ____             _                     
| |    ___   __ _  __| (_)_ __   __ _  |  _ \  ___   ___| | _____ _ __         
| |   / _ \ / _` |/ _` | | '_ \ / _` | | | | |/ _ \ / __| |/ / _ \ '__|        
| |__| (_) | (_| | (_| | | | | | (_| | | |_| | (_) | (__|   <  __/ |     _   _ 
|_____\___/ \__,_|\__,_|_|_| |_|\__, | |____/ \___/ \___|_|\_\___|_|    (_) (_)
                                |___/                                          
```
## Docker Run Command:

This command will run **alpine** container if the image is present locally **but** if not then docker will automatically pull docker/alpine image from docker hub (By default docker is configured to pull from docker hub).

```shell
$ sudo docker run alpine

Unable to find image 'alpine:latest' locally
latest: Pulling from library/alpine
aad63a933944: Pull complete 
Digest: sha256:b276d875eeed9c7d3f1cfa7edb06b22ed22b14219a7d67c52c56612330348239
Status: Downloaded newer image for alpine:latest
 
```
Clearly in my case the image was not present locally so docker pulled it from library/alpine. 
Note : Alpine is a minimal linux for a Docker.

## Docker ps Command:

It is used for listing all the running containers in the system it also shows the basic information about them like CONTAINER ID, IMAGE, CREATED and few more .. 
By Default it shows only the running containers.

```shell
$ sudo docker ps // default case

$ sudo docker ps -a // list all containers 

```
## Docker stop Command:

It is used to stop a running container. From **docker ps** we will get a container id or container name used int the command to stop a container.

```shell
$ sudo docker stop "CONTAINER ID or Container Name"
```
On the succesfull execution of command we get the name of container printed as a output.

## Docker Rm - Remove Command:

If we don't want this container lying around and aquire our physical memory, We use **docker rm** command to permanently remove these exited or unsed containers.

```shell
$ sudo docker rm -f "CONTAINER ID"

// -f for doing it forcefully

```   

## Docker images Command:

It lists all the images of containers present locally in your machine

```shell
$ sudo docker images //-list all images present

```
## Docker rmi command:

It is used to remove an image which we no longer plan to use .. but remember you must ensure remove or stop all the running containers linked to it

```shell
$ sudo docker rmi nginx

``` 

## Docker pull Command:

It is used to directly pull the images from docker hub without running it .. if our image is already present locally then it check for any updates. 

```shell
$ sudo docker pull nginx
```

## Docker exec Command:

It is used for executing a command or a specific task in a container. 

```shell
$ sudo docker exec <NAME of CONTAINER> cat etc/hosts

// will display the contents of /etc/hosts of that container
```

## Port Mapping in docker: 

```shell
$ docker run -p 80:5000 <application name>
```

We are routing the traffic of our port 80 to the 5000 port of docker container 

we can access all data of port on https://192.168.1.5:80

-p is used as a switch for port mapping docker
 
so you can run as many application on docker and map them to as many ports in docker containers

## Docker volume mapping:

```shell
$ docker run -v /opt/datadir:/var/lib/mysql <mysql container name>
```

-v is used to mount this data volume externally so that if we do **rm or stop** in containers then none of the data gets lost it will be redirected every time there is an update in time stamp of the data in container directory

## Docker logs command

```shell
$ docker logs <name of container>
```

docker logs will display current logs of the container 
 
## Docker environment variable mapping in docker 

specify the variable in your application and pass it everytime on command line for any change you want to incorporate in your docker application 

```shell
docker run -e App_colour="blue" <application name>
```

here -e is used to pass variable value into the container application file

## Docker Inspection command:

```shell
$ docker inspect <name of the container>
```

Inspect command is used to see all the details of a Docker Containers, Images, Objects and Services like its id, name, path, args and all other states and mounting options.sla

For results of some objects to be in more human readble output format you can provide a "--pretty" flag. 








































