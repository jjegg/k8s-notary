# Notary k8s yaml

Notary is a service that signs docker images. For sercurity this can be useful as it can establish integrity within your running cluster and enforce rules that only allow signed images to run.

More information around Notary
https://docs.docker.com/notary/getting_started/

## Prerequisites 
Update `notary/server-deployment.yaml` with a custom image that contains certificates for signing the images.

## Deployment
`kubectl apply -f notary-k8s/. -n yournamespacehere`