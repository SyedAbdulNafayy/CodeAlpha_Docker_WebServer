# CodeAlpha Docker Web Server

## Project Overview
Deployed a custom static website using Nginx inside a Docker container.

## Technologies Used
- Ubuntu 22.04
- Docker Engine
- Nginx
- HTML and CSS

## Project Structure
- Dockerfile
- README.md
- site/index.html

## Build Docker Image
sudo docker build -t codealpha-webserver:1.0 .

## Run Container
sudo docker run -d --name codealpha-web -p 8080:80 codealpha-webserver:1.0

## Access Website
http://localhost:8080

## Monitoring
sudo docker ps

sudo docker stats --no-stream

sudo docker logs codealpha-web

## Health Check
sudo docker inspect --format='{{.State.Status}}' codealpha-web

curl -I http://localhost:8080

## Project Outcome
Successfully deployed and monitored an Nginx web server using Docker.
