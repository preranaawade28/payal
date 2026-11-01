#!/bin/bash

#----------------------- update
sudo apt update
sudo apt install fontconfig openjdk-21-jre

#---------------------install jenkin pkg
sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2026.key
echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null

#---------------------VERIFY installation
sudo apt update
sudo apt install jenkins
sudo systemctl status jenkins
