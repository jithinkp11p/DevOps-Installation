
# Install SonarQube.



## Pre-Requisites:

```bash
  Docker and Docker-Compose should be installed 
```

Run the below commands to deploy the SonarQube as container 

```bash
docker run -dit --name sonarqube 9000:9000 sonarqube:lts-community
