# Docker Compose Demo

This project demonstrates how to run multiple containers using Docker Compose.

## Overview

Docker Compose allows developers to define and manage multi-container applications using a single configuration file.

In this project, two services are defined:

- Nginx → Web server
- Redis → Cache service

Both containers are started together using a docker-compose.yml file.

## Technologies Used

- Docker
- Docker Compose
- Nginx
- Redis
- Linux

## Project Structure

docker-compose-demo
│
├── docker-compose.yml
└── README.md

## docker-compose.yml

version: "3"

services:
  web:
    image: nginx
    ports:
      - "8082:80"

  redis:
    image: redis

## Run the project

Start containers:

docker compose up -d

Check running containers:

docker ps

Access the web server:

http://localhost:8082

Stop containers:

docker compose down

## Learning Outcome

- Understanding Docker Compose
- Running multiple containers
- Container orchestration basics
- Managing services using YAML configuration
