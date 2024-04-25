
# Install SonarQube.



## Pre-Requisites: Install Docker 

```bash
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable" -y
sudo apt update -y
apt-cache policy docker-ce -y
sudo apt install docker-ce -y

sudo usermod -aG docker $USER && newgrp docker

```

Run the below commands to deploy the SonarQube as container 

```bash
docker run -dit --name sonarqube -p 9000:9000 sonarqube:lts-community
