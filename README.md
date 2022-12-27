[![CircleCI](https://dl.circleci.com/status-badge/img/gh/angeljudgement/udacity-4/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/angeljudgement/udacity-4/tree/main)

## Operationalize a Machine Learning Microservice API
This Microservice Project's a part of the Udacity Cloud DevOps Engineer Nanodegree

## Project Overview

Deploy a containerized application based on Python to serve the purpose of predict housing prices through API calls. By utilizing a pre-trained sklearn model,
the application is compromised to produce quality data for analytics team.

### Project Tasks

The goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications,
including:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

## Files & Explaination

* Dockerfile - Setup steps to create docker image
* Makefile - Setup environment and export function to run in commandline
* app.py - Python App, base code of prediction
* make_prediction.sh - Send API and receive response
* run_docker.sh - Setup steps to build and run docker locally
* upload_docker.sh - Setup steps to push docker to docker hub
I.E: https://hub.docker.com/repository/docker/stevejks/mydocker-nguyen
* run_kubernetes.sh - Setup steps to run app on kubernetes
* .circleci/config.yml: CircleCI configuration file for C

---

## Setup the Environment

* Create a virtualenv and activate it
```bash
# Python 3.7 is required
# Check python version: which python3
python3 -m venv <your_venv>
source <your_venv>/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl
