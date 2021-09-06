# Docker Cheat Sheet
## Stop all containers
```
sudo docker stop $(sudo docker ps -a -q)
``` 
## Delete all containers
```
sudo docker rm $(sudo docker ps -a -q)
```

## Delete images

### Remove dangling images. 
A dangling image is one that is not tagged and is not referenced by any container.
```
sudo docker images prune
```

### Remove unused images, not just dangling ones
To remove all images which are not used by existing containers
```
sudo docker images prune -a
```



