# Docker_Essential_Cheats
<p align="center">
<image src="https://github.com/DonAlahakoon/Docker_Cheats/assets/89693545/b14e0085-370c-416c-95c6-fa733cddebad" width=500 />
</p>
  
1. Pulling an image from the repository

```markdown
docker pull <name_of_the_image>
```

2. To build an image from a Dockerfile
```markdown
docker build -t <image_name> .
```
> [!NOTE]
> Here ```.``` (optional) means current folder and ```-t``` (optional) is used to tag the image id. Both are optional.

3.  List all local images
```markdown
docker images 
```
4. Delete an image.
```markdown
docker rmi <image_name> 
```
5. Remove all unused images
```markdown
docker image prune
```
6. Publishing an image into Docker
```markdown
docker push <username>/<image_name> 
```
7.  Running a container
```markdown
docker run -t -d -p <host_port>:<container_port> --name <name_of_the_container> <image_name>
```
> [!IMPORTANT]
> ```-t``` tag (optional) is used to tag,<br>
> ```-d``` detach (optional) to run in the background not to show log details and terminal detach from running container,<br>
> ```-p <host_port>:<container_port>``` publish (optional) binding container port to the localhost.


8. To open the shell inside the running container
```markdown
docker exec -it <container_name> sh
```
9.  Check all the running containers
```markdown
docker ps 
```
10. List the containers that ran and exited successfully.
```markdown
docker ps -a 
```
11. Pings application
```markdown
docker localhost
```
12. Stops one or more running containers
```markdown
docker stop
```
> [!TIP]
> To stop all running containers
> ```markdown
> docker stop $(docker ps -q)
> ```

13.To remove a container
```markdown
docker container rm 
```

14.  To see how much memory using by the containers
```markdown
docker stats 
```
15. Creates a tag for a target image that refers to a source image
```markdown
docker tag
```
16. Start the docker daemon
```markdown
docker -d 
```
