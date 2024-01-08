# How to Publish an image to docker HUB ?

- Login to docker
```bash
    docker login
```
- To publish run this command
```bash
    docker tag image_name username/image_name
    # example
    docker tag react-docker iamsidar07/react-docker
    # default tag will be :latest
```
- To push to the docker hub
```bash
    docker push username/image_name
    # example
    docker push iamsidar07/react-docker
```