# Docker Image

- Build an Image from a Dockerfile
```bash
    docker build -t image_name path_to_dockerfile
    # example
    docker build -t myapp .
```
- List all local images
```bash
    docker images
    # example
    docker images ls
```
- Pull an image from docker hub
```bash
    docker pull image_name:tag
    # example
    docker pull ngnix:latest # latest is default tag
```
- Remove a local image
```bash
    docker rmi image_name:tag
    # example
    docker rmi myapp:latest
    # OR
    docker rm [image_name/image_id]
    # example
    docker rm myapp
    # or
    docker rm 2sd
```
- Tag an image
```bash
    docker tag source_image:tag new_image:tag
    # example
    docker tag myapp:latest myapp:v1
```
- Push an image to Docker hub
```bash
    docker push image_name:tag
    # example
    docker push myapp:v1
```
- Inspect details of an image
```bash
    docker image inspect image_name:tag
    # example
    docker image inspect myapp:v1
```
- Save an image to tar archive
```bash
    docker save -o image_name.tar image_name:tag
    # example
    docker save -o myapp.tar myapp:v1
```
- Load an image from a tar archive
```bash
    docker load -i image_name.tar
    # example
    docker load -i myapp.tar
```

- Purne unused iamges
```bash
    docker image purne
```