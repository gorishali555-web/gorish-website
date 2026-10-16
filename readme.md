# GORISH Website

A personal portfolio website and end-to-end DevOps CI/CD project.

## Technologies
- HTML5 and CSS3
- Git and GitHub
- GitHub Actions
- Docker and Docker Hub
- AWS EC2
- Nginx

## CI/CD Pipeline

Code Push -> GitHub Actions -> Docker Build -> Docker Hub -> AWS EC2

## Deployment

Pushing code to the main branch triggers the deployment workflow.

## Required GitHub Secrets

- DOCKERHUB_USERNAME
- DOCKERHUB_TOKEN
- EC2_HOST
- EC2_USER
- EC2_SSH_KEY

## Local Docker Test

Build the image:

docker build -t gorish-website .

Run the website:

docker run -d --name gorish-local -p 8080:80 gorish-website

Open http://localhost:8080
