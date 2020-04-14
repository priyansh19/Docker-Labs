# Constructing Custom Docker Images for Production Environment:

In this Excersise we will see how to construct your own docker image. 

Open your text editor and make a file "Dockerfile"

Similar to this - [Link]()

Once done save the file and buld your docker container using this command:

```shell
docker build Dockerfile -t priyansh19/custom-html-app
```

Now Let's Understand the structure of Dockerfile we built

Docker files contains a specific format that docker can understand.

It contains two thing i.e:

- INSTRUCTION: It is written in CAPS in the left of the Dockerfile

- ARGUEMENT: It is written in th eright portion of the Dockerfile

I have pushed this image to my public docker registry [link]() 

It contains a sample application in html





