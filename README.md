
## Introduction

This repository contains k8 deployment files for deploying [food-ordering-system](https://github.com/muditshukla3/food-ordering-system) application and 3 node kafka cluster using confluent kafka.

#### Kafka Deployment
Run the following command from helm folder to run 3 node kafka cluster on k8.
```
helm install local-confluent-kafka helm/cp-helm-charts --version 0.6.0
```
TODO: Update the command to create kafka topics.

### Postgres Deployment
Run the following command to deploy postgres as k8 service.
```
kubectl apply -f postgres-deployment-local.yml
```
TODO: Update the deployment file to use persistent volumes.
### Application Deployment
Run the following command to deploy all services in k8 cluster.
```
kubectl apply -f application-deployment-local.yml
```