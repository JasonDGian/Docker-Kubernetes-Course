# 📌 Docker Installation
Docker can be installed on **macOS**, **Windows**, and **Linux**, with each operating system having specific requirements that must be met before installation.

## 🔹 Learning about system requirements.
Depending on your device's specifications, you will need to install either **Docker Desktop** or **Docker Toolbox**:   
- **Docker Desktop**: This is the 'standard' version for devices that meet the system requirements.
- **Docker Toolbox**: An alternative for devices that do not meet the requirements for Docker Desktop.

>[!tip]
>To learn about Docker's requirements access the ![official documentation](https://docs.docker.com/desktop/install/mac-install/).

<!-- h2>
<img  height="20px" src="https://github.com/user-attachments/assets/3f88a71f-b453-4490-9f70-d4defb6c5b01"> MacOS.</h2 -->

<h2><img  height="20px" src="https://github.com/user-attachments/assets/9e139738-eb29-4406-9579-8a433053d15e"> Installing on Windows.</h2>
   
For windows machines, the installation is different depending on the OS version. **Windows Home** will have a different installation procedure compared to **Windows Pro**. This is important because Home Edition will require **WSL - Windows Subsistem Linux**, while Proffesional Edition will only require Hyper-V.

> [!IMPORTANT]
> The **Hyper-V** and **Containers** features must be propperly enabled to install Docker Desktop on Windows.
> To enable Hyper-V on Windows follow this link. [Enable Hyper-V fast guide](https://github.com/JasonDGian/Docker-Kubernetes-Course/blob/main/1.2-enable-hyper-v.md)

<table>
   <tr>
      <td>   
         After assuring WSL and Hyper-V are enabled and functional we can procceed with the installation process through the installation wizard.   
        Download the relevant version of <strong>Docker Desktop</strong> from the <a href="https://docs.docker.com/desktop/install/windows-install">official website</a> and follow the steps.   
        Once the installation is finished, if needed, enable the automatic docker service startup.   
      </td>
      <td width="30%">
         <img align="right" src="https://github.com/user-attachments/assets/1a874241-8741-497e-bb2f-bf910d83daf2">
      </td> 
   </tr>
</table>


   
<br/>
   
<h2><img height="20px" src="https://github.com/user-attachments/assets/c51b89c4-c0bf-4e72-86f0-db15c6236101"> Linux  </h2> 
    
The Linux operating system **natively supports** containers and the associated technology, you can either install **Docker Desktop** like in Windows and Mac or directly install the **Docker Engine**.
For more information about the differences between the two check out [docker components](https://github.com/JasonDGian/Docker-Kubernetes-Course/blob/main/1.1-docker-components.md).

**Installing Docker Desktop**
Docker Desktop for Linux provides a user-friendly graphical interface that simplifies the management of containers and services. It includes Docker Engine as this is the core technology that powers Docker containers. Docker Desktop for Linux also comes with additional features like Docker Scout and Docker Extensions.

### ▫️ Disabling native Docker Engine.
On Linux, a Docker Engine instance can run concurrently with a Docker Desktop instance, this can cause issues.Disabling the system's Docker Engine will avoid these issues and even provide a better resource management and experience.

**Check if the service is enabled**
```bash
sudo systemctl status docker
```

Use the following command to stop the Docker Engine service:
```bash
sudo systemctl stop docker docker.socket containerd
sudo systemctl disable docker docker.socket containerd
```

### ▫️ Docker context.
The Docker CLI can be used to interact with multiple Docker Engines. For example, you can use the same Docker CLI to control a local Docker Engine and to control a remote Docker Engine instance running in the cloud. Docker Contexts allow you to switch between Docker Engines instances.

When installing Docker Desktop, a dedicated "desktop-linux" context is created to interact with Docker Desktop. On startup, Docker Desktop automatically sets its own context (desktop-linux) as the current context. This means that subsequent Docker CLI commands target Docker Desktop. On shutdown, Docker Desktop resets the current context to the default context.

Use the `docker context ls` command to view what contexts are available on your machine. 
**The active context is marked with `*`**

```bash
docker context ls
NAME            DESCRIPTION                               DOCKER ENDPOINT                                  ...
default *       Current DOCKER_HOST based configuration   unix:///var/run/docker.sock                      ...
desktop-linux                                             unix:///home/<user>/.docker/desktop/docker.sock  ...
```

**To select a context use the following command:**   
`docker context use <docker-context-name>`

**Example:**
```bash
docker context use desktop-linux
desktop-linux
Current context is now "desktop-linux"
```

## Installation on Arch-based distros.
1. Install gnome terminal.
2. Download the packages.
3. Install the packages.
4. Start the application.

1. Install gnome-terminal.
```bash
 sudo pacman -S gnome-terminal
```
2. Download the Docker binaries.   
Docker does not have an Arch package repository. Binaries not included in the package must be installed manually before installing Docker Desktop. Download the latest Arch package from the [release notes](https://docs.docker.com/desktop/release-notes/).

3. Install the package.     
Install the downloaded package with any possible dependency needed.
```bash
sudo pacman -U path-to-package
```
![imagen](https://github.com/user-attachments/assets/471bca2c-3616-4b4c-97b6-f8cbf1ed56c9)
**By default, Docker Desktop is installed at /opt/docker-desktop.**

4. Start Docker
This can be done either by terminal or by GUI.
![imagen](https://github.com/user-attachments/assets/3e1d9d5c-af2f-4f53-907f-ce4b4f725980)

For the installation follow the [official resources](https://docs.docker.com/desktop/install/linux-install) .  

## 🔹 Confirm the success of the installation.
To check if Docker successfully installed, open a terminal within your system, no matter which one, and type `docker`. A list of possible command switches will appear on scren, otherwise, if you encounter an error message something must have gone wrong during the installation process.
   
![docker command](https://github.com/user-attachments/assets/cabb9f65-42f1-495a-9f42-e085180ed99c)

--- 

# 📌 Create your first container.

>[!TIP]
> By installing `Prettier`and `Docker` plugins on Visual Studio Code you will have a better experience while writing Docker configuration files.
>   
> <img width="380px" src="https://github.com/user-attachments/assets/4a0e7fa1-bcf1-416d-854b-b47926a3c4f3">
> <img width="380px" src="https://github.com/user-attachments/assets/28dd9556-84bc-4163-b67e-b499317b1899">


![imagen](https://github.com/user-attachments/assets/f66ed9f4-1ebb-4a52-ada0-883396da9955)












