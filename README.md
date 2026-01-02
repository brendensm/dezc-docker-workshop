# dezc-docker-workshop
workshop codespaces

What is Docker?
allows you to create an isolated "container"
does not affect the host system
everytime we run a docker container -- it is made from an image
image has a complete snapshot of everything 
stateless -- does not prevserve state -- nothing saved, back to square 1

some images (like python:3.13.11-slim) has things preinstalled (in this example, python)
 can add the flag --entrypoint=bash to go into bash (not just python)

docker doesnt preserve state typically... 
technically you can find it (not great practice)

docker ps -a to see containers

> docker rm `docker ps -aq`
remove old ones

mounting volumes to a docker container