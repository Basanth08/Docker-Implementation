# Docker Examples

This directory contains practical examples of Docker implementations that I've created during my learning journey.

## 📁 Contents

### Python Flask Application (`python-docker-app/`)
A simple containerized Python Flask web application demonstrating:
- Basic Flask web application
- Dockerfile creation
- Requirements.txt for dependency management
- Port mapping and containerization

**Features:**
- `/` - Hello Docker message

**To run:**
```bash
cd python-docker-app
docker build -t flask-app .
docker run -p 8000:5000 flask-app
```

## 🚀 Getting Started

Each example includes:
- Complete source code
- Dockerfile
- Instructions for building and running

## 📚 Learning Objectives

These examples demonstrate:
- Basic containerization concepts
- Dockerfile creation
- Port mapping
- Environment variables
- Multi-container setup with Docker Compose

## 🔧 Technologies Used

- **Python Flask** - Web framework
- **Docker** - Containerization
- **Docker Compose** - Multi-container orchestration
- **PostgreSQL** - Database
- **Redis** - Caching layer 