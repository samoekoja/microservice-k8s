[![samoekoja](https://circleci.com/gh/samoekoja/microservice-kubernetes.svg?style=svg)](https://app.circleci.com/pipelines/github/samoekoja/microservice-kubernetes)

# Project Summary
During the course of this project, I was able to: 
* Operationalise a ML Microservice API
* Containerize it with Docker
* Deploy the containerized application
* Upload the image to Dockerhub
* Deploy it with Kubernetes
* Achieve CircleCI Integration

# Project running 
## Setting a python 3.7 virtual environment and activating it
python3 -m venv ~/.devops

source ~/.devops/bin/activate

## Installing the necessary dependencies
make install

## Running the main application
python app.py

## Run in Docker: 
./run_docker.sh
## Run in Kubernetes: 
./run_kubernetes.sh

# Files Summary

* .circleci/config.yml: CircleCI configuration file.
* app.py: The python application
* requirements.txt: Required Python packages to run the application
* Makefile: Installation and Linting Config
* Dockerfile: Docker Container config
* upload_docker.sh: Tag and upload the Docker image to DockerHub
* run_docker.sh: Runs the containerized application
* run_kubernetes.sh: Runs the application on a Kubernetes cluster
* make_prediction.sh: Makes a prediction call to the running Application
* output_txt_files/docker_out.txt: Console output from make_prediction.sh for run_docker.sh
* output_txt_files/kubernetes_out.txt Console output from  make_prediction.sh for run_kubernetes.sh

# Links

[Output Text Files](https://github.com/samoekoja/microservice-kubernetes/output_text_files/)

[CircleCI](https://app.circleci.com/pipelines/github/samoekoja/microservice-kubernetes)
