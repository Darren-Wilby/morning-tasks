# Docker

## 1. What is containerization, and how does it differ from virtualization?

​Containerisation is a lightweight form of virtualization that allows you to package and isolate applications and their dependencies into self-contained units called containers. Containers share the same operating system kernel with the host but have their isolated file systems and runtime environments.

Virtualization involves running multiple virtual machines (VMs) on a single physical host. Each VM includes a full operating system and runs its applications. Virtualization provides strong isolation but consumes more resources compared to containers because each VM needs its OS kernel.

## 2. Why is containerization important in modern software development and deployment?

-   ​Containers encapsulate an application and its dependencies, making it easy to move and run the same application across different environments (development, testing, production) and cloud providers.
-   Containers share the host OS kernel, reducing resource overhead compared to VMs. They start quickly and are highly scalable.
-   Containers ensure that the application runs consistently regardless of the underlying infrastructure.
-   Containers facilitate automation, enabling faster development cycles and easier deployment.

## 3. What is the difference between an image and a container in Docker?

-                                     An image is a lightweight, standalone, and executable package that includes the application code, runtime, libraries, and dependencies needed to run a piece of software. Images are read-only and provide a blueprint for creating containers.
-   A container is an instance of an image that runs as a process on a host machine. Containers are isolated from each other and the host system, providing a consistent and reproducible runtime environment for applications.

## 4. Can you give an example of a situation where you might choose to use Docker containers in a software development project?

In a software development project, you might use Docker containers to:

-   Isolate microservices: Run different parts of your application stack in separate containers for better isolation and scalability.
-   Create development environments: Ensure that developers work with consistent and reproducible development environments by using containers with predefined configurations.
-   Streamline CI/CD pipelines: Use containers to build, test, and deploy applications consistently across different stages of the development lifecycle.

## 5. If you were tasked with explaining Docker to someone who has never heard of it before, how would you describe it in a few sentences?

-   Docker allows you to build containers which contain everything needed to run an application.
-   Docker makes it easier for developers to package, share, and run applications in a predictable way, whether on their laptops or in the cloud.​

## Extension

​
Fill in this cheat sheet throughout the day to help and remind you understand how to use Docker commands
​
| Command | Description |
| :-----: | ----------- |
| ps | It shows you the containers that are currently active on your Docker host |
| images | Lists the Docker images available on your system. Images are the templates for creating containers |
| pull | Download Docker images from a remote registry, such as Docker Hub, to your local system |
| build | Build a Docker image from a Dockerfile and a specified build context. It creates a custom image based on your configuration |
| run | Create and start a new Docker container from an image |
| stop | Stop a running container |
​
| Flag | Description  
|:------:|---------------------------------------------------
| -a | (--all): When used with docker ps, it shows all containers, including stopped ones. By default, docker ps only displays running containers. |
| -d | (--detach): When used with docker run, it runs the container in the background and prints the container ID. |
| -t | (--tty): When used with docker run, it allocates a pseudo-TTY (terminal) for the container. It's often used when you want to interact with the container's command line. |
| -p | (--publish): When used with docker run, it specifies port mapping. It allows you to map a port on your host machine to a port in the container, making the container's service accessible from the host. |
​
Below is an example of a how you might format a docker command. (In documentation having something wrapped in square brackets [] denotes that it is optional to provide this in the command)
​

```bash
docker run [OPTIONS] <IMAGE[:TAG|@DIGEST]> [COMMAND] [ARG...]
```
