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


## Pull image
```
sudo docker pull eu.gcr.io/dpa-gke-workshop/hello-app-tom:v1
sudo docker images
```
