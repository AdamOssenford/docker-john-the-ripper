# THIS IS AN AUTOMATED BUILD OF JOHN THE RIPPER FOR DOCKERHUB
This is the github repository for https://hub.docker.com/r/adamoss/john-the-ripper

USAGE
=========  
## YOU NEED TO MOUNT THE FILE YOU WISH TO CRACK USING -v
### DOCKER CANNOT MAGICALLY READ THE HOST FILE SYSTEM SO PLEASE REMEMBER TO PASS THE MOUNTS TO THE CONTAINER

``` 
docker run -it -v `pwd`/yourfiletocrack:/crackme.txt adamoss/john-the-ripper /crackme.txt
```
### in the above example docker is mounting your file to crack inside the container as /crackme.txt then it passes /crackme.txt to john

```
docker run -it -v `pwd`/yourfiletocrack:/crackme.txt adamoss/john-the-ripper /crackme.txt
```

## if you want to enter without launching john 
```
docker run -it adamoss/john-the-ripper /bin/bash
```
