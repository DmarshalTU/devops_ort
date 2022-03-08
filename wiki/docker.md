![](/assets/docker-cover.png)
[Docker Website](https://www.docker.com)


[lab](https://github.com/DmarshalTU/devops_ort/blob/main/labs/docker_lab.md)


# Terminology
## Docker engine (aka Docker):
Docker Engine is an open-source containerization technology for building and
containerizing your applications

![](/assets/servlet.ImageServer.png)

![](/assets/Container-vm-whatcontainer_2.png)



## Docker client:
The Docker client ( docker ) is the primary way that users interact with Docker.
When you use commands such as docker run , the client sends these commands
to dockerd , which carries them out. The docker command uses the Docker API.
The Docker client can communicate with more than one daemon.

![](/assets/AppDesigner_composite_windows_v4.webp)



## Docker image:
A Docker image is a file used to execute code in a Docker container.
Docker images act as a set of instructions to build a Docker container.
Docker images are the bricks of Docker

* Docker images are read only templates
* Images are the application which we run
* Docker images are launched from containers
* Images are pulled from Docker hub/ Container registry
* Each image contain series of layers combined using AUFS


![](/assets/a4254b7670297f798bdadf3ebabc42b1.png)


## Docker container:
A container is a standard unit of software that packages up code and all its
dependencies, so the application runs quickly and reliably from one computing
environment to another.

A Docker container image is a lightweight, standalone, executable package of
software that includes everything needed to run an application: code, runtime,
system tools, system libraries and settings

* Standardized packaging for software and dependencies
* Isolated apps from each other
* Share the same OS kernel
* An image instance
* Running as process (Linux: Cgroups, Namespaces)
* We can have multiple container running the same image
* Containers can share information
* Exit when the process stops


![](/assets/y5a5yat0scob.png)


## Docker File:
A Dockerfile is a text document that
contains all the commands a user
could call on the command line to
assemble an image.

Using docker build users can create
an automated build that executes
several command-line instructions in
succession.

![](/assets/main-qimg-648201449c17a4cfe876432b19bf8ad8.png)


## Docker Hub / Registry:
A Docker registry is a storage and distribution system for named Docker images
available in different tagged versions.

Users interact with a registry by using docker push and pull commands.

Registry can be private or public.

[DockerHub Website](https://hub.docker.com)


## Cheat Sheet:
![](/assets/dockercheatsheet8.png)
