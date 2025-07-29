sudo apt update
sudo apt  install docker.io -y
sudo usermod -aG docker $USER
newgrp docker
docker run -d --name sonar -p 9000:9000 sonarqube:lts-community
