# End-to-End Text_Summarizer Project

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity
4. Update the configuration manager in src config
5. Update the components
6. Update the pipeline
7. Update the main.py
8. Update the app.py

# How to run?
### STEPS

Clone the repository

```bash
https://github.com/WillNovus/Text_Summarizer
```

### STEP 01 - Create a conda environment after opening the repository

```bash
conda create -n text python=3.8 -y
```
```bash
conda activate text
```

### STEP 02 - Install the requirements
```bash
pip install -r requirements.txt
```

```bash
#Finally run the following command
python app.py
```
Now,
```bash
open up your local host and port
```

```bash
Author: Will Gabriel
Role:   Machine Learning Engineer
Email:  gabrielwill666@gmail.com
```


# AWS-CICD-Deployment-with-GitHub-Actions

## 1. Login to AWS Console

## 2. Create IAM user for deployment

    #with specific access

    1. EC2 Access: It is a virtual machine

    2. ECR: Elastic Container registry to save your docker image in aws.

    #Description: About the deployment

    1. Build docker image of the source code
    
    2. Push your docker image to ECR

    3. Launch your EC2

    4. Pull your image from ECR to EC2

    5. Launch your docker image in EC2

    #Policy

    1. AmazonEC2ContainerRegistryFullAccess

    2. AmazonEC2FullAccess

# 3. Create ECR Repo to store/save docker image
    - Save the URI: 566373416292.dkr.ecr..us-east-1.amazonaws.com/catdog

## 4. Create EC2 machine (Ubuntu)

## 5. Open EC2 and install docker in EC2 Machine:

    #Optional

    sudo apt-get update -y

    sudo apt-get upgrade

    #required

    curl -fsSL https://get.docker.com -o get-docker.sh

    sudo sh get-docker.sh

    sudo usermod -aG docker ubuntu

    newgrp docker

## 6. Configure EC2 as self-hosted runner
    setting>actions>runner>new self hosted runner> choose os> then run command one by one

## 7. Setup github secrets:
    AWS_ACCESS_KEY_ID =
    AWS_SECRET_ACCESS_KEY = 
    AWS_REGION = us-east-1
    AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr..us-east-1.amazonaws.com
    ECR_REPOSITORY_NAME = simple-app

