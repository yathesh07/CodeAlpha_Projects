# CodeAlpha Docker Web Server

## Project Overview

This project demonstrates the deployment of a web server using Docker as part of the CodeAlpha DevOps Internship.

## Objectives

* Learn Docker containerization
* Deploy a web server inside a Docker container
* Understand Docker images and containers
* Manage container lifecycle
* Explore deployment best practices

## Technologies Used

* Docker
* Nginx
* HTML

## Project Structure

CodeAlpha_Docker_WebServer

├── Dockerfile

├── index.html

└── README.md

## Build Docker Image

docker build -t codealpha-webserver .

## Run Docker Container

docker run -d -p 8080:80 --name codealpha-container codealpha-webserver

## Access Application

http://localhost:8080

## Author

Yathesh V

Aspiring Full Stack Developer & AI Developer
