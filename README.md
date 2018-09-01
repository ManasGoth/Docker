# Docker
Docker from scratch

Terminologies: 
1> Docker is not a virtual machine. It's all about isolation.
2> Image : It is a class definition
3> Container: It's a running image. It's an object created from the class (image)/ instance of a class.
4> Host: It's the machine which docker is running. If on a windows machine , we are running docker on a linux container then Windows is the host. 

<br> Docker Image is a set of files which has no state, whereas Docker Container is the instantiation of Docker Image. In other words, Docker Container is the run time instance of images. </br>

<br>Commands</br>
$> docker run -it --rm ubuntu /bin/bash

docker -> cli
run -> command
-it & --rm -> options
ubuntu /bin/bash -> arguments

$> docker run [OPTIONS] IMAGE [COMMANDS] [ARG...]

$> docker run -it ubuntu /bin/bash
root> ls

<br>To see a list of all running container</br>
$>docker ps
<br>To see the list of all containers </br>
$>docker ps -a
$>docker ps -all
<br>To start the container</br> 
$>docker start <container id>
<br>To attach to a container  









