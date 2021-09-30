[![CircleCI](https://circleci.com/gh/YassminAbubakr/DevOps_Microservices_FinalPrj/tree/main.svg?style=svg)](https://circleci.com/gh/YassminAbubakr/DevOps_Microservices_FinalPrj/tree/main)


## Project Overview

In this project, i used the skills that i acquired in this course to operationalize a Machine Learning Microservice API. 
By Applying Docker & Kubernetes concepts to predict housing prices in Boston .
Docker Technology uses the Linux kernel system so the processes can run independently .
Kubernetes is an open-source platform that manages containerized workloads and services that can simplify the configurationand automation.
### Project Tasks

Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

### Required Files in Repo
- .circleci/config.yml : Defines an automated testing environment; CircleCI uses a YAML file to identify how you want your testing environment set up and what tests you want to run.  
- app.py : file contained the pre-trained model prediction. 
- Dockerfile : The Dockerfile contains all the required commands to build an image from CMD. 
- make_prediction.sh : This script is responsible for sending some input data to your containerized application via the appropriate port. Each numerical value in here represents some feature that is important for determining the price of a house in Boston. 
- Makefile : it includes instructions for environment setup,lint and tests. 
- requirements.txt : contain all the lib dependencies that need to be installed. 
- run_docker.sh : has a list of all docker commands to build & run the docker image that is built previously in Dockerfile. 
- run_kubernetes.sh : This is used to deploy your application on the Kubernetes cluster, This assumes you have a local cluster configured and running. This script should create a pod with a name specified. 
- upload_docker.sh : This script upload the built image to docker. This will make it accessible to a Kubernets cluster.

## Setup the Environment

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### CircleCi Link
   https://app.circleci.com/pipelines/github/YassminAbubakr/DevOps_Microservices_FinalPrj

