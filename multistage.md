# Multi Stage Sample

## Connect to VM instance
Use Webbrowser or SSH

## Build container
cd to 03-multistage-go
```
docker build -t single-stage -f Dockerfile.single .
docker build -t multi-stage -f Dockerfile.multi .
```

## Images
```
docker images
```

## Run
```
docker run single-stage
docker run multi-stage
```
