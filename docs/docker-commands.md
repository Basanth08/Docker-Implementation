# Docker Commands I've Learned

## Basic Container Commands

### Running Containers
```bash
# Run a container
docker run hello-world

# Run container with port mapping
docker run -p 8000:5000 my-app

# Run container with environment variables
docker run -e key=value my-app

# Run container interactively
docker run -it <image-name>
```

### Managing Containers
```bash
# List running containers
docker ps

# List all containers (including stopped)
docker ps -a

# Start a stopped container
docker start <container-name>

# Stop a running container
docker stop <container-name>

# Remove a container
docker rm <container-name>
```

## Image Commands

### Working with Images
```bash
# List all images
docker images

# Pull an image from Docker Hub
docker pull [image]

# Build an image from Dockerfile
docker build -t my-app .
```

### Interactive Container Access
```bash
# Execute command in running container
docker exec -it <container-name> bash

# Access container shell
docker exec -it <container-name> bash
```

## Docker Compose Commands

### Managing Services
```bash
# Start services in background
docker compose up -d

# Stop and remove services
docker compose down
```

## Commands I Use Regularly

```bash
# Container Management
docker run hello-world                    # Run first container
docker ps -a                             # List all containers
docker start/stop <container-name>       # Control container lifecycle
docker rm <container-id>                 # Remove containers

# Image Operations
docker pull [image]                      # Download images from Docker Hub
docker images                            # List all local images
docker build -t my-app .                 # Build custom images

# Interactive Container Access
docker exec -it <container-name> bash    # Access container shell
docker run -it <image-name>              # Run image interactively

# Port Mapping & Environment Variables
docker run -p 8000:5000 <image-name>     # Port mapping
docker run -e key=value <image-name>     # Environment variables

# Docker Compose
docker compose up -d                     # Start services in background
docker compose down                      # Stop and remove services
``` 