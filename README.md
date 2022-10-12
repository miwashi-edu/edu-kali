# edu-kali

[Kali](https://www.kali.org/)
[Installera hacker verktyg i kali](https://www.kali.org/docs/containers/official-kalilinux-docker-images/)

## Docker

[Images](https://www.kali.org/docs/containers/official-kalilinux-docker-images/)

## Videos

[Kali](https://www.youtube.com/watch?v=lZAoFs75_cs)  
[Kali Linux in Docker](https://www.youtube.com/watch?v=JGgu8jVTejk)  
[Docker For Pentesting And Bug Bounty Huntingy](https://www.youtube.com/watch?v=5G6tA8Q9AuQ)  
[]()  
[]()  
[]()  

## ctrl-characters
[GeeksForGeeks](https://www.geeksforgeeks.org/control-characters/)  
[Wikipedia](https://en.wikipedia.org/wiki/Control_character)  

## Instructions

```bash
docker pull kalilinux/kali-rolling:latest
docker run --name kali  -t -i kalilinux/kali-rolling

# I Kali
apt update
apt -y install kali-linux-headless

# ctrl-d (end of file) för att avsluta.
````

### Configure Kali

```bash

```

### Run again if stopped
```bash
docker ps -a
CONTAINER ID   IMAGE                       COMMAND                  CREATED          STATUS                      
62b674a706ee   kalilinux/kali-rolling      "bash"                   29 minutes ago   Exited (0) 3 minutes ago
docker start 62b674a706ee 
docker attach 62b674a706ee
```

### Do ower cleanup

```bash
docker ps -a
CONTAINER ID   IMAGE                       COMMAND                  CREATED          STATUS                      
62b674a706ee   kalilinux/kali-rolling      "bash"                   29 minutes ago   Exited (0) 3 minutes ago
docker container rm -f 62b674a706ee
docker image rm -f kalilinux/kali-rolling

````
