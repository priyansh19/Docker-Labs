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
##1. Docker **Run** Command:

This command will run **nginx** container if the image is present locally **but** if not then docker will automatically pull docker/nginx image from docker hub (By default docker is configured to pull from docker hub).

```shell
$ sudo docker run nginx

Unable to find image 'nginx:latest' locally
latest: Pulling from library/nginx
c499e6d256d6: Already exists 
74cda408e262: Already exists 
ffadbd415ab7: Already exists 
Digest: sha256:282530fcb7cd19f3848c7b611043f82ae4be3781cb00105a1d593d7e6286b596
Status: Downloaded newer image for nginx:latest
``` 
Clearly in my case the image was not present locally so docker pulled it from library/nginx.
