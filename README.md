# DevOps-Project
The project contains terraform file which creates EC2 instance with ssh-key so we can log in later. <br><br>
Once the machine is started, Jenkins is installed automatically. <br><br>
The terraform file creates also an ECR (Elastic Container Registry) where I will keep the docker images. <br><br>
The Dockerfile will build the application from Github.<br><br>
Multibranch pipeline is used in Jenkins to build Jenkinsfile if it is available in the branch.<br><br>
The Jenkinsfile includes the following steps:
- builds the Dockerfile
- push it into the ECR
- deploys the helm chart in Kubernetes by passing the tag dynamically
# 
