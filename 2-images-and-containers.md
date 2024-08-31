# 📌 Docker images and containers.

## 🔹 What is a docker container.
A Docker container is a lightweight, standalone, executable package that includes everything needed to run a piece of software or application, including the code, 
runtime, system tools, libraries, and settings. Containers ensure that software runs reliably when moved from one computing environment to another. This software unit packages code and all its necessary dependencies to run correctly. **This allows developers to distribute and run 'ready to use' applications and server-like utilities.**

## 🔹 What is a docker image.
An image can be defined as a template or a blueprint for a docker instance. A docker image not only contains the code and instructions to execute to create the container but it also contains the code and tools that the container will later use.

## 🔹 Container vs Image.
A Docker image is like a blueprint or template that defines how a container should be built. It is static and read-only. In contrast, a Docker container 
is a runnable instance of an image, which means it is the live environment where the application runs. 
   
Containers are created from images and can be started, stopped, moved, and deleted. While the image remains unchanged, the container can have a dynamic state, including changes to files or running processes.

<img width="48%" src="https://github.com/user-attachments/assets/bd44d695-73ae-4e95-b0f2-64d56f815fe7">
<img width="48%" src="https://github.com/user-attachments/assets/cfa1564d-b715-4737-a2b7-579ec085ef40">
