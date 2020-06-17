# ElastAlert-Docker

This Dockerfile will build a Docker image for Elastalert. This image is compatible with the accompanying Helm chart for Kubernetes.

## Building Locally

To build, install Docker and then run the following command:
```
docker build . -t elastalert
```

## Kubernetes

See the Helm chart [README.md](chart/elastalert/README.md) for information on installing this application into an existing Kubernetes cluster.

## run 

docker run -d -v /home/rules/config.yaml:/opt/config/elastalert_config.yaml -v /home/rules/:/home/rules jertel/elastalert-docker
