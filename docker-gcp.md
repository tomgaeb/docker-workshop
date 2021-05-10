## build and run

``` 
gcloud config set run/region europe-west3

gcloud builds submit --tag gcr.io/dpa-gke-workshop/myweb:v1
gcloud run deploy mywev-v1 --image gcr.io/dpa-gke-workshop/myweb:v1 --platform managed
```


