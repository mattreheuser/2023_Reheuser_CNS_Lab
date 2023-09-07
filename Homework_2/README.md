# 7330: Computer and Network Security Homework 2 
## Matthew Reheuser 
#### 2023.09.06 <p>&nbsp;</p>

# Finding Docker Containers 
## itzg/minecraft-server
I looked at Minecraft server offered on dockerhub. There is not an organization behind the container rather it is a community of dedicated gamers supporting it, there are almost 200 contributors on Github. There are a handful of enviromental variables that can be used such as declaring a modpack to run on the server, 

## Python
This is an offical docker image. The organization behind this container is the docker community with licensing from Python. The Python docker created a local development environemtn to be used for development in Python. Some of the options you can use with the docker are the version of Python and the location of where you want your Python file to be run from. This box is unique because it can easily create a development environment.<p>&nbsp;</p>   

# Adding Docker Container  
## kalilinux/kali-rolling   
The docker I added to my docker-compose configuration was Kali Linux's kali-rolling, which is the offical Kali Linux docker image. The organization behind the container is Offensive Security who are the creators of Kali Linux. Offensive Security creates open source projects with a focus in information security and penetration testing. With this install of Kali Linux there are no real options while the container is running because the docker has no tools or applications installed. However once running a command to get the basic kali programs the container can be used to crack passwords, intercept network packets, and numerous other penetration testing tactics.    

# Images  
![Broadcasting](./pictures/10.9.0.1_broadcasting.png)  
First off the way the seed box is set up, 10.9.0.1 is reserved and cannot have a container using that address. Therefor the intial picture we were supposed to go off of from lab 2 would not work, so I used 10.9.0.2 for my attacker container.<p>&nbsp;</p>
![Docker Version](./pictures/dockerVersion.png)  
After resolving that problem, I had to update my version of docker. This was causing problems running apt on any of the containers because the version of docker running on the machines version 19.03.08 reached its end of life date 2 years and 8 months ago, so I realized that very few docker boxes will work with that.<p>&nbsp;</p>
![dockps](./pictures/dockps.png)  
This is me showing my attacker container on the configuration as a part of the dockps command. <p>&nbsp;</p>
![Kali](./pictures/KaliRoot.png)  
I was able to get into the Kali Linux container and utilize it running within my configuration. The root matches the value that corresponds with the container in the upper picture.

