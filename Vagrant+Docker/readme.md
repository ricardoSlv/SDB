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

# Run Docker swarm leader
sudo docker swarm init --advertise-addr 10.128.0.15:2377

# Join Docker Swarm 
sudo docker swarm join --token TOKENHERE

# Check swarm on leader
sudo docker node ls

# Launch swarm on leader
sudo docker stack deploy -c docker-compose.yml sdb

# Inspect service
docker serve in pretty-print

# Upscale/Downscale swarm
sudo docker service scale sdb_web=1