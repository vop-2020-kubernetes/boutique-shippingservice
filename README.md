**NOTE:** This repository is part of an example deployment, the original application you can find here: https://github.com/GoogleCloudPlatform/microservices-demo

This deployment has been adapted to fit our GitOps flow.
The original application has been split, creating a git repository per microservice.

Check https://github.com/vop-2020-kubernetes/boutique-ci-cd for more info about our project.




# Shipping Service

The Shipping service provides price quote, tracking IDs, and the impression of order fulfillment & shipping processes.

## Local

Run the following command to restore dependencies to `vendor/` directory:

    dep ensure --vendor-only

## Build

From `src/shippingservice`, run:

```
docker build ./
```

## Test

```
go test .
```
 
