# Run nginx

## Connect to VM instance
Use Webbrowser or SSH

## Start nginx container

### Locally
```
sudo docker run -it --rm -d -p 8080:80 --name web nginx
curl localhost:8080
```

### Different port
```
sudo docker run -it --rm -d -p 80:80 --name web nginx
```

### Without name
```
sudo docker run -it --rm -d -p 80:80 nginx
```

## Create own nginx image
change to directory 01-images

``` 
sudo docker build -t webserver .
```

## Links
https://www.docker.com/blog/how-to-use-the-official-nginx-docker-image/


