---
created:
  - 2024-03-09 10:24
tags:
  - docker
---
# Fundamentals

![[docker-img-1.png]]

### What is Docker?
Simplified, Docker is a way to package software so it can run on any hardware

##### DockerFile
A blueprint for building a docker image
- A Dockerfile is **a text document that contains all the commands a user could call on the command line to assemble an image**.

##### Image
A template for docker containers
- A Docker image is **a file used to execute code in a Docker container**. Docker images act as a set of instructions to build a Docker container, like a template. Docker images also act as the starting point when using Docker. An image is comparable to a snapshot in virtual machine (VM) environments.

##### Container
A running process
- A Docker container image is **a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings**.

- A dockerfile helps set up and reproduce the environment.
- The development environment is saved as a immutable snapshot known as an image.
- images can be uploaded in public/private registries.
- Users can download images to create a container which is a running process of that image.  One image file can spawn multiple times in multiple places.