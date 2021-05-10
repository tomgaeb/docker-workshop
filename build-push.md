# Build and push
Login in Cloud Shell

## Clone Google Repo
```
git clone https://github.com/GoogleCloudPlatform/kubernetes-engine-samples.git
cd kubernetes-engine-samples/hello-app
```

## Build image
```
docker build -t eu.gcr.io/dpa-gke-workshop/hello-app-tom:v1 .
```


## Push image
```
docker push eu.gcr.io/dpa-gke-workshop/hello-app-tom:v1
```

## Connect to VM instance
Use Webbrowser

## Google Auth
``` 
gcloud auth login
gcloud config set project dpa-gke-workshop

gcloud config set compute/region europe-west3
gcloud config set compute/zone europe-west3-c


gcloud container clusters create gke-tom --num-nodes=1
sudo gcloud auth configure-docker
```


## Pull image
```
sudo docker pull eu.gcr.io/dpa-gke-workshop/hello-app-tom:v1
sudo docker images
```
