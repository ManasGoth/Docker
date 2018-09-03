# Docker
Docker from scratch

Terminologies: 
1> Docker is not a virtual machine. It's all about isolation.
2> Image : It is a class definition
3> Container: It's a running image. It's an object created from the class (image)/ instance of a class.
4> Host: It's the machine which docker is running. If on a windows machine , we are running docker on a linux container then Windows is the host. 

<br> Docker Image is a set of files which has no state, whereas Docker Container is the instantiation of Docker Image. In other words, Docker Container is the run time instance of images. </br>

<br>Commands</br>
$> docker run [OPTIONS] IMAGE [COMMANDS] [ARG...]

$> docker run -it --rm ubuntu /bin/bash
<br>docker -> cli </br>
<br>run -> command </br>
<br>-it & --rm -> options </br>
<br> ubuntu -> image </br>
<br> /bin/bash -> arguments </br>

<br>To see a list of all running container</br>
$>docker ps
<br>To see the list of all containers </br>
$>docker ps -a
$>docker ps -all
<br>To start the container</br> 
$>docker start <container id>
<br>To attach to a container</br>
$>docker attach <container id>
  
<br>=======RUNNING THE HELLO WORLD CONTAINER========</br>
<br>When you run the command "Docker run hello-world"  </br>

<br>PS C:\Users> docker run hello-world</br>
<br>Unable to find image 'hello-world:latest' locally</br>
<br>latest: Pulling from library/hello-world</br>
<br>9db2ca6ccae0: Pull complete</br>
<br>Digest: sha256:4b8ff392a12ed9ea17784bd3c9a8b1fa3299cac44aca35a85c90c5e3c7afacdc</br>
<br>Status: Downloaded newer image for hello-world:latest</br>

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/engine/userguide/

<br>============RUNNING THE ubuntu CONTAINER==========</br>

<br>PS C:\Users\Manas.Goth.GEP> docker run -it ubuntu bash</br>
<br>Unable to find image 'ubuntu:latest' locally</br>
<br>latest: Pulling from library/ubuntu</br>
<br>124c757242f8: Pull complete</br>
<br>2ebc019eb4e2: Pull complete</br>
<br>dac0825f7ffb: Pull complete</br>
<br>82b0bb65d1bf: Pull complete</br>
<br>ef3b655c7f88: Pull complete</br>
<br>Digest: sha256:72f832c6184b55569be1cd9043e4a80055d55873417ea792d989441f207dd2c7</br>
<br>Status: Downloaded newer image for ubuntu:latest</br>
<br>root@f03e000f29ef:/# ls</br>
<br>bin   dev  home  lib64  mnt  proc  run   srv  tmp  var
boot  etc  lib   media  opt  root  sbin  sys  usr</br>

$ docker stop <container name>
  1. The docker client takes the input and sends it to the docker daemon
  2. The docker daemon then traces the container and passes on the command
  3. The container listens to the command and passes it to the process in the conatiner and says it to exit. 
  
  More Commands:
  1.docker run -it -d --rm --name ubuntu1 ubuntu bash
    -it -> interactive
    -d -> detach ( when container starts it's not automatically attached to the terminal)
    --rm -> when container stops , remove it automatically
    --name -> give a name to the conatiner . In this case "ubuntu1"
    [ubuntu] -> is the image name 
    [bash] -> is the argument
 <br>Check Logs </br>
 $> docker logs <container name>
 
 <b> BUILDING IMAGES </b>
    
  
  
  
  



