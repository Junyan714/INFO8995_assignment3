# Junyan Zhang's Containers Prototype

## Overview
This project demonstrates container orchestration using Docker Compose. It includes:
1. A web service that responds with a sentence from a configuration file.
2. A load balancer (NGINX) to distribute traffic to the web service.

## Prerequisites
- Docker
- Docker Compose

## Features
- Container orchestration with Docker Compose.
- Health checks to ensure service readiness.
- Network isolation using a custom bridge network.
- Environment variables for configuration flexibility.

## Best Practices
Environment variables are used for flexibility.
Health checks ensure the web service is ready before the load balancer starts.
A custom network ensures container isolation.

## How to Run
1. Clone the repository.
2. Navigate to the project directory.
3. Run the following command to start the service:
docker-compose up
4. The load balancer will be available at `http://localhost:8080`.

## Files
- `web_service/app.py`: Python Flask web service.
- `web_service/config.txt`: Configuration file with the sentence.
- `load_balancer/nginx.conf`: NGINX configuration for load balancing.

## Stopping the Service
To stop the service, press `CTRL+C` and then run:

