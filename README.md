# Project4

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/w01000001ssim/DevOps_Microservices/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/w01000001ssim/DevOps_Microservices/tree/main)

## A summary of the project

This project involved the deployment of a pre-trained scikit-learn ML model as a Python Flask Microservice API. Code quality was validated via linting, containerization was achieved through Docker, and deployment was managed through Docker and Kubernetes. Model predictions were made and the code was improved with enhanced logging. The entire project was version-controlled in a Github repository with CircleCI integration to verify successful build and test execution.

## Instructions on how to run the Python scripts and web app

### Setup the Environment

* Create a virtualenv and activate it:
    
    ```bash
    python3 -m venv ~/.devops
    source ~/.devops/bin/activate
    ```

* Run `make install` to install the necessary dependencies

### Running the Scripts

* Run `python run_docker.sh` to build the Docker image and run the container

* Run `python run_kubernetes.sh` to run the container in Kubernetes

### Making a Prediction

* Run `./make_prediction.sh` to make a prediction

## Files in the repository

* `app.py`: A Flask application that provides housing price predictions through API calls.
* `Dockerfile`: Dockerfile to build the image
* `Makefile`: Makefile with commands to setup and install the project, lint and test the code
* `run_docker.sh`: Script to build the Docker image and run the container
* `run_kubernetes.sh`: Script to run the container in Kubernetes
* `make_prediction.sh`: Script to make a prediction