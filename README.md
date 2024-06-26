# Softy-Pinko Docker Project

This repository showcases a series of Docker-based projects designed to help you practice and understand containerization, the fundamentals of Docker, and microservices architecture. Docker is a robust platform that enables developers to bundle applications into containers—self-contained units that include the application code, runtime, system tools, libraries, and settings necessary for the application to run.

## Project Overview

In this project, we will build a comprehensive infrastructure for an application using Docker. The key objectives include setting up a reverse proxy, implementing load balancing, and managing multiple services within Docker containers.

### High-Level Architecture

The project's architecture involves the following components:

- **Reverse Proxy/Load Balancer**: Acts as the entry point to the application.
- **API Servers**: Two instances to handle backend logic.
- **Front-End Server**: Serves static content to the users.
- **Traffic Management**: Uses a round-robin algorithm to evenly distribute requests among the API servers.

## Prerequisites

- Install Docker Desktop on your local machine. Instructions are available on Docker's official website.
- Have a basic understanding of Docker concepts and commands.

## Tasks

### Task 0: Create Your First Docker Image

- Create a Docker image based on the latest Ubuntu.
- Update APT and upgrade all installed software.
- The Docker image should echo "Hello, World!" when executed.

### Task 1: Back-End

- Develop a backend service using Python3 and Flask.
- Ensure the Dockerfile handles Python dependencies via pip.

### Task 2: Front-End

- Set up a front-end service to serve static content using Nginx.
- Configure Nginx to listen to incoming requests on a specified port.

### Task 3: Connecting the Front-End and Back-End

- Enable communication between the front-end and back-end services.
- Ensure the front-end can dynamically display data fetched from the back-end.

### Task 4: Simplify with Docker Compose

- Use Docker Compose to manage the multi-container application.
- Define services, build contexts, Dockerfiles, images, and ports in a `docker-compose.yml` file.

### Task 5: Proxy Server

- Implement a proxy server using Nginx.
- Route requests to the appropriate service based on the request URL using a JavaScript proxy setup in your HTML file.

### Task 6: Horizontal Scaling

- Scale the application horizontally by adding multiple instances of the API server.
- Manage these instances using Docker Compose.

## Repository Details

- **GitHub Repository**: atlas-softy-pinko-docker
- **Directory Structure**: Each task has its own directory under the root of the repository.

By following these tasks, you'll learn how to build a scalable and maintainable multi-service application using Docker and Nginx.
