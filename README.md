[![CircleCI](https://circleci.com/gh/benita-ekene/Dev.Ops.svg?style=svg)](https://circleci.com/gh/benita-ekene/Dev.Ops)

## Project Overview

In this project, you will operationalize a Machine Learning Microservice API. 
You are given a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on.

### Project Tasks

The goal of this project is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

**The final implementation of the project will showcase your abilities to operationalize production microservices.**

---

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

**Standalone:**
app.py contains the web app built using flask framework.

python app.py

**Run in Docker:**
run_docker.sh contains the script to run the app in the docker.

./run_docker.sh

**Run in Kubernetes:**
run_kubernetes.sh contains the script to run app in the Kubernetes.

./run_kubernetes.sh

## Verify that application is running
make_prediction.sh contains the script to check the predictions.

./make_prediction.sh

### Upload to Docker Hub 
upload_docker.sh contains the script to upload the docker image to the Docker Hub.

./upload_docker.sh

## Kubernetes Steps
Setup and Configure Docker locally
Setup and Configure Kubernetes locally
Create Flask app in Container
Run via kubectl

## Kubernetes Clean Up
kubectl delete deployment.apps/app
kubectl delete svc app

