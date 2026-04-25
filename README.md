#  CI/CD Pipeline for Dockerized Web Application on AWS

##  Live Demo
🔗 http://65.0.30.184

>  Note: The application runs on AWS EC2. If the instance is stopped, the site may not be accessible.


##  Project Overview
This project demonstrates an end-to-end DevOps workflow by deploying a containerized web application using Docker, automating it with CI/CD, and hosting it on AWS EC2.


##  Tech Stack
- Version Control: Git & GitHub
- Containerization: Docker
- CI/CD: GitHub Actions
- Cloud Platform: AWS EC2
- Web Server: Nginx


##  Workflow

Code → GitHub → Docker → Docker Hub → AWS EC2 → Live Website
 

##  Features
- Dockerized web application  
- Automated CI/CD pipeline  
- Deployed on AWS EC2  
- Publicly accessible  
- Lightweight Nginx server  


##  Deployment Steps

### 1. Clone Repository

git clone https://github.com/chaitrarodda/devops-project.git
cd devops-project

### 2. Build Docker Image
docker build -t myproject .

### 3. Run Locally
docker run -d -p 8080:80 myproject

### 4. Push to Docker Hub
docker tag myproject chaitrarodda/myproject
docker push chaitrarodda/myproject

### 5. Deploy on AWS EC2
sudo docker run -d -p 80:80 chaitrarodda/myproject


##  Key Learnings
- Docker containerization  
- CI/CD with GitHub Actions  
- AWS EC2 deployment  
- Networking & security groups  

##  Author
Chaitra Rodda
