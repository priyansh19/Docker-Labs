<p align="center">
 <img width="336" height="270" src="Images/geektechstuff_docker.png">
</p>

This is the beginning of learning Docker from basics. 

**Docker** is a tool which is used to automate the deployments of an application in lightweight containers so that application can work efficiently in different environments 

**Containers** are completely **Isolated Environments** as in they can have their own processes, services
, networking and a lot of things using the **Kernel** of the Host machine. There are various types of containers and Docker uses LXC type of containers.

The **Biggest difference** between Containers and Virtual Machines is that the container are quiet different as they all shares one kernel and the virtual machines have a seperate kernel running in each and the containers don't use the principle of virtualization its just using a kernel for different operating os.

### Is Docker Useful for GUI Applications?

Docker could help solve some challenges associated with desktop apps. For example, it could enable truly platform-agnostic app packages. We’ve come a long way since the days when you had to compile your app from source to make it run on your system. But most installation packages available today are still tied to a particular Linux distribution or version of Windows. With Docker, it finally would be possible to have a single package format for installing a given application on any Linux or Windows system.

### Why do you need Docker ? 

* Compatibility and Dependency issues over long term use of a same environment.
* Long time to setup similar environment for a new user
* There are different environments with different dependencies for development/Testing and for production as well 

### Features:

 - Multiple containers can run on the same hardware
 - high productivity as it uses the same kernel as of the os 
 - maintains isolated applications so that thier dependencies do clash with each other
 - Ouick and easily configurable virtual machines
 - We can share our images with other users very easily 

## Installation of Docker in Linux :

To install docker in Linux type the following set of commands

```shell 
sudo apt-get install docker docker.io

// To verify your installation try this -

sudo docker run hello-world

// You will see a message "Hello from Docker!"
```

## Objectives :

- Getting Started With Docker
- Learning Concepts 
- Learning Commands
- Fun Excercises

## Excersises :

1. Learning about Docker and its architechture [link]()

2. Docker Basic Commands [link]()

3. Building your very own first DOCKERFILE [link]()

4. Installing Dependencies in Docker [link]()

5. Configuring Containers [link]()

## Contributions :

As of now we don't accept contributions. It is a fun project so start learning and have fun :+1:

## Author :

Priyansh Gupta
