# Part 2

## Introduction

Now that we have our application packaged as container images, where do they go?

## Description

In this challenge we will be creating and setting up a new, private, Azure Container Registry. This will be the new home of the containers we just created. We will see later on how Kubernetes will pull our images from this registry.

- Login to your ACR
- Push your Docker container images to the ACR
- Use ``` az acr build ``` to build images not local
- List all images in your ACR


## Success Criteria

1. You have deployed your container images to the registry.
2. You can log into the registry and see all images.
