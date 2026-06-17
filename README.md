# Containerized Website Hosting with Docker & Nginx

## Project Overview

This project demonstrates how I containerized and deployed a static educational website using Docker and Nginx.

The primary objective of this project was to gain practical experience with Docker by packaging a front-end web application into a portable container that can run consistently across different environments.

Instead of focusing on website development, this project focuses on the complete containerization workflow, including building Docker images, running containers, exposing ports, and serving static web content through Nginx.

---

## Technologies Used

* Docker
* Nginx
* HTML
* CSS
* JavaScript

---

## Project Structure

```text
Docker-Capstone-Project1/

├── Dockerfile
├── README.md
└── school-website/
    ├── index.html
    ├── css/
    ├── js/
    ├── images/
    └── assets/
```

---

## Docker Implementation

### Dockerfile

A custom Dockerfile was created to:

1. Use an Nginx base image.
2. Copy website files into the Nginx web root directory.
3. Configure the container to serve the static website.
4. Expose the required HTTP port.

### Build Docker Image

```bash
docker build -t educational-website .
```

### Run Docker Container

```bash
docker run -d -p 8080:80 educational-website
```

The website becomes accessible through the mapped host port while being served from inside the container by Nginx.

---

## Docker Concepts Demonstrated

* Building custom Docker images
* Writing Dockerfiles
* Containerizing static web applications
* Using Nginx inside containers
* Port mapping between host and container
* Running containers in detached mode
* Managing container lifecycle
* Image creation and deployment
* Container isolation and portability

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Creating and managing Docker images
* Deploying static websites inside containers
* Understanding the Docker build process
* Working with Nginx as a containerized web server
* Running and managing containers using Docker CLI
* Publishing containerized applications for deployment

---

## Future Improvements

* Multi-stage Docker builds
* Docker Compose integration
* CI/CD pipeline automation
* Deployment to AWS EC2
* Container orchestration using Kubernetes

---

## Author

**Mervin Shaji**

Containerized Website Hosting with Docker & Nginx
