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
sudo docker login akstraining202109.azurecr.io
sudo docker tag hello-app-tom:v1 akstraining202109.azurecr.io/hello-app-tom:v1
sudo docker push akstraining202109.azurecr.io/hello-app-tom:v1
```

## Build with ACR
1. Install Azure CLI and authenticate
```
sudo apt install azure-cli
```

2. Build and push image
```
az acr build --registry akstraining202109 . -t nginx-tom:v2
```


## Run on ACI
Edit name, image and DNS label!
```
az container create --resource-group aks-training-rg --name acr-hello-tom --image akstraining202109.azurecr.io/acr-hello-tom:v1 --dns-name-label aci-demo-tom --ports 80
```


