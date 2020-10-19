# Docker
check docker version
```bash
docker -v
```
pull image from docker host
```bash
docker pull image_name 
```
Run nginx with configure website.
```bash
docker run --name website -v $(pwd):/usr/share/nginx/html:ro -d -p 8000:80 nginx
```
run container with tag
```bash
docker run nginx:lastest
```
run container with tag and in background and port number
```bash
docker run -d -p 8080:80 nginx:lastest
```
stop docker container
```bash
docker stop  port_number
```
List all container
```bash
docker ps -a
```
List all container only id
```bash
docker ps -aq
```
remove container by id
```bash
docker rm container_id
```
remove all containers
```bash
docker rm $(docker ps -aq)
```
remove all containers by forcing
```bash
docker rm -f $(docker ps -aq)
```
run container with name
```bash
docker run ---name name -d -p 3000:80 nginx:lastest
```
