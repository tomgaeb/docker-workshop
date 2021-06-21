# Build and push
Login in Cloud Shell

## Clone Azure Samples Repo
```
git clone https://github.com/Azure-Samples/acr-build-helloworld-node
cd acr-build-helloworld-node
```

## Build image
```
sudo docker build -t hello-app-tom:v1 .
```

## Run locally
```
docker run -d -p 80:80 helloacrbuild:v1
Navigate to http://(DOCKER VM IP) to view the running application
```

## Push image
```
sudo docker login akstraining202106.azurecr.io
sudo docker tag hello-app-tom:v1 akstraining202106.azurecr.io/hello-app-tom:v1
sudo docker push akstraining202106.azurecr.io/hello-app-tom:v1
```
