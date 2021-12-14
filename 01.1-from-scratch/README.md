# Hello World from scratch

## prep
gcc installieren oder docker build nutzen

## Lokal kompilieren
```
gcc -static -o hello hello-word.c
```



## In einem Container kompilieren
```
sudo docker build -t hellobuild:latest -f DockerBuild .
id=$(sudo docker create hellobuild:latest)
sudo docker cp $id:/hello hello
sudo docker rm $id
./hello
```

## Create and run container
```
docker build -t hello:latest .
docker run hello:latest
```
