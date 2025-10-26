# AtSea Shop Deployment with Docker Swarm

Orchestrating the "AtSea Shop" microservice app using Docker Swarm, focusing on secure configuration management with `Docker Secrets` and `Docker Config`.

## Project Overview

This project involved deploying a multi-container e-commerce application (`AtSea Shop`) on a Docker Swarm cluster.

The primary goal was to move beyond standard environment variables and implement a secure, production-ready configuration strategy.

## Key Technical Implementations
* **Orchestration:** Used `Docker Swarm` to manage the lifecycle of all services (database, app server, reverse proxy).
* **Secure Secrets Management:** All sensitive data (database credentials, payment tokens, SSL keys) were managed as `Docker Secrets`, removing them from the image and compose file.
* **Externalized Configuration:** The `nginx.conf` file for the reverse proxy was managed externally using `Docker Config`, allowing for updates without rebuilding the image.
* **Custom Images:** Built custom Docker images from source `Dockerfiles` for each service.

## Key Technologies
* Docker & Docker Swarm
* Docker Compose (`docker-compose.yml`)
* `Docker Secrets`
* `Docker Config`
* Nginx (as Reverse Proxy)
* PostgreSQL

## Report
The full technical report, `docker-compose.yml` file structure, and deployment steps are available in the `پروژه AtSea Shop با Docker Swarm.pdf` file.
