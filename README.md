# Docker_Essential_Cheats
<p align="center">
<image src="https://github.com/DonAlahakoon/Docker_Cheats/assets/89693545/b14e0085-370c-416c-95c6-fa733cddebad" width=500 />
</p>
1. Pulling an image from the repository

```markdown
docker pull <name_of_the_container>
```

2. List all images
```markdown
docker images 
```
3. Running a container
```markdown
docker run -t -d --name <name_of_the_container> 
```
4. Check all the running containers
```markdown
docker ps 
```
5. List the containers that ran and exited successfully.
```markdown
docker ps -a 
```
6. Pings application
```markdown
docker localhost
```
7. Stops one or more running containers
```markdown
docker stop
```
> [!TIP]
> To stop all running containers
> ```markdown
> docker stop $(docker ps -q)
> ```
8. To see how much memeory using by the containers
```markdown
docker stats 
```
9. 
