# What is Docker ?

**Docker** is a tool used to automate the deployments of an application in lightweight containers so that application can work efficiently in different environments 

<p align='center'>
	<img width="336" height="270" src="~/Images/geektechstuff_docker.png">
</p>

## What are containers ?

**Containers** are completely **Isolated Environments** as in they can have their own processes, services, networking and a lot of things using the **Kernel** of the Host machine. There are various types of containers and Docker uses LXC type of containers.

The **Biggest difference** between Containers and Virtual Machines is that the container are quiet different as they all shares one kernel and the virtual machines have a seperate kernel running in each and the containers don't use the principle of virtualization its just using a kernel for different operating os.

Docker can't run Windows OS with different kernel on the same hardware with linux containers because unlike Hypervisors, Docker is not meant to run and virtualise different Operating Systems and kernels on same hardware. The main aim of Docker is to package, maintain an environment and to ship them and to run them anywhere and as many times as you want.

## Is Docker Useful for GUI Applications?

Docker could help solve some challenges associated with desktop apps. For example, it could enable truly platform-agnostic app packages. We’ve come a long way since the days when you had to compile your app from source to make it run on your system. But most installation packages available today are still tied to a particular Linux distribution or version of Windows. With Docker, it finally would be possible to have a single package format for installing a given application on any Linux or Windows system.

## Why do you need Docker ? 

* Compatibility and Dependency issues over long term use of a same environment.
* Long time to setup similar environment for a new user
* There are different environments with different dependencies for development/Testing and for production as well 

# Architechture of Docker



