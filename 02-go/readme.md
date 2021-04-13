# Build and start container with Cloud Run (Without Docker) 😀


```
go mod init
```

```
gcloud builds submit --tag gcr.io/k8s-workshop-intern/helloworld-NAME
gcloud run deploy --image gcr.io/k8s-workshop-intern/helloworld-NAME --platform managed
```


Links
https://cloud.google.com/run/docs/quickstarts/build-and-deploy#go