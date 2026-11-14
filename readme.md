# Create Helm Chart for Microservices

**Technologies used:** Kubernetes, Helm

## Project Description

Create 1 shared Helm Chart for all microservices, to reuse common Deployment and Service configurations for the services.

One generic chart (`charts/microservice`) deploys every microservice, with a separate values file per service in `values/`. All releases can be installed at once with `install.sh` or `helmfile.yaml`.

## Screenshots

![Installing the email service](images/emailservice.png)
*Installing `emailservice` from the shared chart, with its 2 pods running.*

<br>

![Installing the recommendation service](images/recommendation.png)
*Installing `recommendationservice` from the same chart with a different values file.*

<br>

![Running pods](images/pods.png)
*Pods for both services running, deployed from one shared chart.*
