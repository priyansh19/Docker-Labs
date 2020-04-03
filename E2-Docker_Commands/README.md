## Basic Docker Commands

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
1. This command will run **nginx** container if the image is present locally **but** if not then docker will automatically pull docker/nginx image from docker hub (By default docker is configured to pull from docker hub).

```shell
$ sudo docker run nginx
``` 
