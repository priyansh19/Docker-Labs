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

It is used for listing all the running containers in the system it also shows the basic information about them like 

```shell
$ sudo docker ps


