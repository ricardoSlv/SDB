# Build Image
docker build -t my/tomcat . 

# Run Image
docker run -p 8080:8080 -d -t my/tomcat

# List docker images
docker image ls

# List Docker containers
docker ps

# List Docker Running containers
docker ps -a

# Stop Docker Container
docker stop container

# Remove Docker Container
docker rm container

# Docker compose
docker compose up -d web

# Copy files to vagrant vm
scp -r docker_env/ vagrant@10.0.0.101:~/
