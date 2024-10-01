# Microservices_Project-
@ Creating a Pipeline to Deploy Application code from Github to a web server running as a container

# Pre-requisites-
1)Jenkins Server with all dependencies installed (including Maven)
2)Ansible Master
3)Install Docker inside an Ec2 servers [ Webserver and Ansible Master ]
4)Add users of Ansible Master and Remote Servers to the docker Group
5)usermod -aG <groupname> <username>

# Steps-
1)Create a Git Repo
2)Establish connectivity between Jenkins and Ansible Master
3)Add Ansible Server details to Jenkins
4)Establish connectivity between Ansible Master and Webserver
5)Create a Maveb job for package building
6)Identify the code to convert to package using Maven
7)Create a Docker image and push the image to the Docker hub repo
8)Executing ansible playbook to create a container inside the web server.

# Project Diagram-
DEVELOPER (PUSH CODE) >> GIT HUB >> JENKINS & MAVEN SERVER >> ANSIBLE MASTER >> DOCKER (WEBSERVER & DOCKER HUB) 
