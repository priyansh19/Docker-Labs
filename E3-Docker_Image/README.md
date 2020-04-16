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






```

I have pushed this image to my public docker registry [link]() 

It contains a sample application in html





