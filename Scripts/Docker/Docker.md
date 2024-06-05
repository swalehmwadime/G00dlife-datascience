#   Docker README
`Docker is a platform for developing,shipping and running applications.` It provides a way to package applications and their dependencies into standardized units called containers. These containers can then be deployed across different environments, whether it's a developer's laptop, a testing environment, or a production server, with consistent behavior regardless of the underlying infrastructure.

## Key Concepts in Docker
![Docker snap](https://github.com/swalehmwadime/G00dlife-datascience/blob/main/Data%20Analytics/docker1.png)

### 1. Container
A lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, and dependencies. Containers are isolated from each other and from the host system.

### 2. Dockerfile
A text file that contains instructions for building a Docker image. These instructions specify the base image to use, any additional software to install, environment variables, and other configuration settings.

### 3. Image
An immutable snapshot of a Docker container. Images are created from Dockerfiles and can be stored in registries such as Docker Hub or a private registry. They serve as the basis for creating and running containers.

### 4. Registry
A centralized repository for storing and distributing Docker images. Docker Hub is the default public registry maintained by Docker, but organizations can also set up private registries for internal use.

### 5. Docker Engine
The core component of Docker that manages containers. It includes a server daemon, a REST API for interacting with the daemon, and a command-line interface (CLI) for interacting with Docker.

### 6. Compose
A tool for defining and running multi-container Docker applications. Compose uses a YAML file to define the services, networks, and volumes that make up an application, making it easy to manage complex application architectures.

## Installing Docker

To install Docker on your system, follow the instructions for your operating system:

- **Windows:** [Install Docker Desktop on Windows](https://docs.docker.com/desktop/install/windows-install/)
- **MacOS:** [Install Docker Desktop on Mac](https://docs.docker.com/desktop/install/mac-install/)
- **Linux:** [Install Docker Engine on Linux](https://docs.docker.com/engine/install/)

## Basic Docker Commands

### List All Docker Images
```sh
docker images
```

### List All Containers
```sh
docker ps
```

### List All Containers (Running and Stopped)
```sh
docker ps -a
```

## Working with Docker Images and Containers

### Pulling a Docker Image
To download a Docker image, use the `docker pull` command:
```sh
docker pull <image-name>:<version/tag>
```
Example:
```sh
docker pull nginx:1.27
```

### Creating and Running a Container
To create and run a container from an image:
```sh
docker run <image-name>:<version/tag>
```
Example:
```sh
docker run nginx:1.27
```

To run a container in detached mode (in the background):
```sh
docker run -d <image-name>:<version/tag>
```
Example:
```sh
docker run -d nginx:1.27
```

### Viewing Container Logs
To view the logs of a running container:
```sh
docker logs <container-id>
```

### Stopping a Container
To stop a running container:
```sh
docker stop <container-id or container-name>
```

### Port Binding in Docker
To bind a port on your local machine to a port in the container, use the `-p` flag:
```sh
docker run -d -p <local-port>:<container-port> <image-name>:<version/tag>
```
Example:
```sh
docker run -d -p 80:80 nginx:1.27
```
Access the container on `localhost:80`.

## Image Versioning
Docker images can have multiple versions or tags. It is important to specify the correct version when pulling or running an image. The default version is usually `latest` if no version is specified.

### Example with Nginx
For demonstration purposes, you can use the Nginx web server:
```sh
docker pull nginx:1.27
docker run -d -p 80:80 nginx:1.27
```
Access the web server at [http://localhost](http://localhost).

## Important Links

- **Definition/Introduction:** [Docker Overview](https://learn.microsoft.com/en-us/training/modules/intro-to-docker-containers/2-what-is-docker)
- **How Docker Images Work:** [Docker Images](https://learn.microsoft.com/en-us/training/modules/intro-to-docker-containers/3-how-docker-images-work)
- **How Docker Containers Work:** [Docker Containers](https://learn.microsoft.com/en-us/training/modules/intro-to-docker-containers/4-how-docker-containers-work)
- **When to Use Docker Containers:** [When to Use Docker](https://learn.microsoft.com/en-us/training/modules/intro-to-docker-containers/4-how-docker-containers-work)
- **Summary/Overview:** [Docker Documentation](https://learn.microsoft.com/en-us/training/modules/intro-to-docker-containers/6-summary)

## Additional Resources
Learn [Docker](https://www.youtube.com/watch?v=pg19Z8LL06w) in less than an hour. Video

