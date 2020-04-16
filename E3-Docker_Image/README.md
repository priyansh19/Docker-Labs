# Constructing Custom Docker Image:

In this Excersise we will see how to construct your own docker image. 

Open your text editor and make a file "Dockerfile" [Like](https://github.com/priyansh19/Docker/blob/master/E3-Docker_Image/Dockerfile) this     

Once done save the file and buld your docker container using this command:

```shell
sudo docker build . -t priyansh19/custom-html-app
```

Now Let's Understand the structure of Dockerfile we built

Docker files contains a specific format that docker can understand.

It contains two thing i.e:

- Instruction : It is written in CAPS in the left of the Dockerfile. It is a set of instructions which docker can understand

- Arguement : It is written in th eright portion of the Dockerfile. They are the arguements passed for cunstructing docker environment.

```shell
## Sample Dockerfile
## It is must that dockerfiles should start with FROM Instruction
FROM ubuntu:latest
## RUN is used to install dependencies in containers
RUN apt-get update
## COPY is used to copy files from our local system to new docker container
COPY . /opt/source-code/
## ENTRYPOINT allows us to run a command when the image boots up
ENTRYPOINT EXAMPLE=/opt/source-code/ex.py python run
```

Docker uses a layered architechture in building the docker images, each layer only stores the changes from the previous layer hence it helps us to restart the build process of the image from where it fails.

I have pushed this image to my public docker registry [link](https://hub.docker.com/repository/docker/priyansh19/custom-html-app) 

It contains a sample application in html





