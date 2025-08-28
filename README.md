# end-to-end-Book_recommendation_system

## workflow

- config.yaml
- entity
- config/configuration.py
- components
- pipeline
- main.py
- app.py

#how to Run?

Clone the repository

https://github.com/akashsingh79036/End-to-End-Book-Recommender-System.git

```bash
https://github.com/akashsingh79036/end-to-end-Book_recommendation_system.git
```
###step 01- create a conda environment after opening the repository

```bash
conda create -n books python=3.7.10 -y
```

```bash
conda activate books
```

###step 02- install the requirements
```bash
pip install -r requirements.txt
```

how run
```bash
streamlit run app.py
```

# Streamlit app Docker Image Deployment

#1. Login with your AWS console and launch an EC2 instance

#2. Run the following commands

Note: Do the port mapping to this port:- 8501

Note: Do the port mapping to this port :-8501

```bash
sudo apt-get update -y

sudo apt-get upgrade

#Install Docker

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

git clone "your-project"

docker build -t akashsingh79036/end-to-endpoint:latest .

docker images -a

docker run -d -p 8501:8501 akashsingh79036/end-to-endpoint

docker ps

docker stop container_id

docker rm $(docker ps -a -q)

docker login

docker push akashsingh79036/end-to-endpoint:latest

docker rmi akashsingh79036/end-to-endpoint:latest

docker pull akashsingh79036/end-to-endpoint
