# Microservices_Project
Creating a Pipeline to Deploy Application code from Github to a web server running as a container

Pre-requisites-
Jenkins Server with all dependencies installed (including Maven)
Ansible Master
Install Docker inside an Ec2 servers [ Webserver and Ansible Master ]
Add users of Ansible Master and Remote Servers to the docker Group
usermod -aG <groupname> <username>

Steps-
Create a Git Repo
Establish connectivity between Jenkins and Ansible Master
Add Ansible Server details to Jenkins
Establish connectivity between Ansible Master and Webserver
Create a Maveb job for package building
Identify the code to convert to package using Maven
Create a Docker image and push the image to the Docker hub repo
Executing ansible playbook to create a container inside the web server.

Project Diagram-

DEVELOPER (PUSH CODE) >> GIT HUB >> JENKINS & MAVEN SERVER >> ANSIBLE MASTER >> DOCKER (WEBSERVER & DOCKER HUB) 
