# Build and push
Login in Cloud Shell

## Clone Google Repo
```
git clone https://github.com/GoogleCloudPlatform/kubernetes-engine-samples.git
cd kubernetes-engine-samples/hello-app
```

## Build image
```
docker build -t eu.gcr.io/k8s-workshop-intern/hello-app-tom:v1 .
```


## Push image
```
docker push eu.gcr.io/k8s-workshop-intern/hello-app-tom:v1
```

## Connect to VM instance
Use Webbrowser

## Google Auth
``` 
gcloud auth login
gcloud config set project k8s-workshop-intern
sudo gcloud auth configure-docker
```


## Pull image
```
sudo docker pull eu.gcr.io/k8s-workshop-intern/hello-app-tom:v1
sudo docker images
```
