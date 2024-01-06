# Docker Container
- Run a container from an image
```bash
    docker run container_name image_name
    # example
    docker run myapp
```
- Run a named container from an image
```bash
    docker run --name container_name image_name:tag
    # example
    docker run --name mycontainer myapp:v1
```
- List all running containers
```bash
    docker ps
```
- List all containers (Including stopped one)
```bash
    docker ps -a
```
- Stop a running container
```bash
    docker stop container_name_or_id
    # example
    docker stop mycontainer
    # or 
    docker stop ajd
```
- Start a running container
```bash
    docker start container_name_or_id
    # example
    docker start mycontainer
    # or 
    docker start ajd
```
- Run a container in interactive mode
```bash
    docker run -it container_name_or_id
    # example 
    docker run -it mycontainer
```
- Run a container in interactive shell mode
```bash
    docker run -it container_name_or_id sh
    # example 
    docker run -it mycontainer sh
```
- Remove stopped container
```bash
    docker rm container_name_or_id
    # example
    docker rm mycontainer
```
- Remove a running container forcefully
```bash
    docker rm -f container_name_or_id
    # example
    docker rm -f mycontainer
```
- Inspect detail of a container
```bash
    docker inspect container_name_or_id
    # example
    docker inspect mycontainer
```
- View container logs
```bash
    docker logs container_name_or_id
    # example
    docker logs mycontainer
``` 
- Pause a running command
```bash
    docker pause container_name_or_id
    # example
    docker pause mycontainer
```
- Unpause a running command
```bash
    docker unpause container_name_or_id
    # example
    docker unpause mycontainer
```