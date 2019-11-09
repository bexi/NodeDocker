# Example project for testing node with docker

## build docker image
docker build -t <your username>/node_docker .

## view docker images
docker images

## run the image (optional port)
docker run -p 49160:8080 -d <your username>/node_docker

## test app
curl -i localhost:49160

## see running containers
docker ps

## see logs
docker logs <container id>

## go inside container
docker exec -it <container id> /bin/bash
