# AtSea Shop Deployment with Docker Swarm

[cite_start]Orchestrating the "AtSea Shop" microservice app using Docker Swarm[cite: 33], focusing on secure configuration management with `Docker Secrets` and `Docker Config`.

## Project Overview

[cite_start]This project involved deploying a multi-container e-commerce application (`AtSea Shop`) on a Docker Swarm cluster[cite: 33, 76].

The primary goal was to move beyond standard environment variables and implement a secure, production-ready configuration strategy.

## Key Technical Implementations
* [cite_start]**Orchestration:** Used `Docker Swarm` to manage the lifecycle of all services (database, app server, reverse proxy)[cite: 36, 76].
* [cite_start]**Secure Secrets Management:** All sensitive data (database credentials, payment tokens, SSL keys) were managed as `Docker Secrets`, removing them from the image and compose file[cite: 34, 53, 55, 57, 58].
* [cite_start]**Externalized Configuration:** The `nginx.conf` file for the reverse proxy was managed externally using `Docker Config`, allowing for updates without rebuilding the image[cite: 33, 59, 63].
* [cite_start]**Custom Images:** Built custom Docker images from source `Dockerfiles` for each service[cite: 65].

## Key Technologies
* [cite_start]Docker & Docker Swarm [cite: 33]
* [cite_start]Docker Compose (`docker-compose.yml`) [cite: 72]
* [cite_start]`Docker Secrets` [cite: 34, 53]
* [cite_start]`Docker Config` [cite: 33, 59]
* [cite_start]Nginx (as Reverse Proxy) [cite: 59, 130]
* PostgreSQL

## Report
The full technical report, `docker-compose.yml` file structure, and deployment steps are available in the `پروژه AtSea Shop با Docker Swarm.pdf` file.
