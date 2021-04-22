### Project 4 Documentation 


## Run Project Locally 

How to install docker - installed via the link provided. For WSL 2, I went into powershell and set default to WSL2. 
My command: wsl --set-version Ubuntu-18.04 2

How to build the container - docker build -t ceg:20 .

How to run the container - docker run -d -p 5000:80 ceg:20

How to view in browser: 127.0.0.1:5000


## Configure AWL CLI 

How I installed - 

First command: curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

Second Command: unzip awscliv2.zip

Third Command: sudo ./aws/install

How to Configure: Use aws configure and then enter the information provided with the project. 

Go into .aws/credentials and put the access keys. Then go into .aws/config and put the region and output (json)


## Command for ECR: 

Command: aws exr create-repository --repository-name ceg3120/w032exo --region us-east-1

## Configure Github secrets

Setting up secrets: go into the github repo and click settings. Scroll down to secrets and then create secrets. Here we named ours AWS_ACCESS_KEY and AWS_SECRET_ACCESS. After that, you would enter in your 2 keys and it would save and be applied to the repo. 

## Configure Github Workflow

Variables to Change: 

MY_AWS_REGION - insert the region - us-east-1
MY_ECR_REPOSITORY - insert my repo - ceg3120/w032exo 
