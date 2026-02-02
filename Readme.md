# Docker Compose – Multi-Container Application

## Overview
This project demonstrates a **multi-container application** using **Docker Compose**.  
It consists of a **web service (Nginx)** and a **database service (MySQL)** managed together using a single configuration file.

---

## Services
- **Web**: Nginx web server exposed on port **9090**
- **DB**: MySQL database using `mysql:8.0` image

---

## Service Interaction
- Web and DB services are orchestrated using Docker Compose
- Services communicate through Docker’s default network
- Database runs as a backend service for the application

---

## Commands Used
```bash
docker-compose up -d
docker-compose ps
docker ps
docker-compose up -d --scale web=2
docker-compose down

## Outcome 
Understood the concept of multi-container applications
Learned how Docker Compose manages multiple services
Gained hands-on experience with service orchestration
Learned how to verify running containers and services
Understood how to stop and clean Docker environments properly
