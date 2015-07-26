## Docker Cheat Sheet

Misc notes on how to make docker do stuff.

### basic

    docker images
    docker ps -a
    docker rm -f <container name>
    docker rmi <image name>
    docker stop
    docker run -it --name <name> <image-name> [command]
    docker exec -it <container name> <command>
    docker exec -it dvt /bin/bash
    docker run -d -p to:from --name <name> <image-name>    
    docker run -d -p 8883:80 --name dvt mhowlett/nginx-datavstime
    
### boot2docker

#### temporary port forwarding:

    boot2docker ssh -vnNTL 8000:localhost:8000

more notes on that here: 

https://github.com/boot2docker/boot2docker/blob/master/doc/WORKAROUNDS.md

#### initializing env

    $(boot2docker shellinit)

### orchestration

#### automated reverse proxy

http://jasonwilder.com/blog/2014/03/25/automated-nginx-reverse-proxy-for-docker/
