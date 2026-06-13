# CodeAlpha Jenkins Remoting Project

## Overview

This project demonstrates Jenkins Remoting using Docker containers as part of the CodeAlpha DevOps Internship.

## Objectives

* Set up Jenkins Controller
* Configure Jenkins Agent Node
* Establish Jenkins Remoting Connection
* Execute distributed builds
* Understand node isolation and remote execution

## Technologies Used

* Jenkins LTS
* Jenkins Inbound Agent
* Docker
* Docker Network

## Architecture

Jenkins Controller
│
▼
Jenkins Agent
│
▼
Build Execution

## Docker Commands

### Create Network

docker network create jenkins

### Run Jenkins Controller

docker run -d --name jenkins-controller --network jenkins -p 8081:8080 -p 50000:50000 jenkins/jenkins:lts

### Run Jenkins Agent

docker run -d --name jenkins-agent --network jenkins jenkins/inbound-agent:latest-jdk21 -url http://jenkins-controller:8080 -secret <SECRET> -name docker-agent

## Results

* Jenkins Controller deployed successfully
* Agent connected successfully
* Jenkins Remoting established
* Distributed build environment created

## Author

Yathesh V

Aspiring Full Stack Developer & AI Developer
