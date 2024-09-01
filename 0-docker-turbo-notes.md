# 📌 Install docker.
To make docker work you need to enable Hyper-V or the official release packages depending on the OS.
## Windows.
- Enable Hyper-V
- Check if PRO or HOME edition.
  - On HOME install WSL2
    
**Install interactively**
1. Download the installer using the download button at the top of the page, or from the release notes.
2. Double-click Docker Desktop Installer.exe to run the installer. By default, Docker Desktop is installed at C:\Program Files\Docker\Docker.
3. When prompted, ensure the Use WSL 2 instead of Hyper-V option on the Configuration page is selected or not depending on your choice of backend.
4. If your system only supports one of the two options, you won't be able to select which backend to use.
5. Follow the instructions on the installation wizard to authorize the installer and proceed with the install.
6. When the installation is successful, select Close to complete the installation process.
7. Start Docker Desktop.

## Linux
Linux can install Docker Engine and work without Docker Desktop.   
**Install Docker Desktop**   
1. Install docker engine (needed for desktop).
2. Install gnome terminal.
3. Download & Install the official released packages
4. Enable services.
5. Start the application.

# 📌 Common use commands.

  ## Build a docker image. 
  Build a container image based on the dockerfile settings.
  Everytime a change is made on the source files a new image must be built to include said changes.
  ```bash
  docker build <path to dockerfile>
  ```  

  ## Creating and stopping Docker instances. 
  Runs the given image creating a container instance based on it.
  ```bash
  docker run <imagename>
  ```
  Stops the container with said ID.
  ```bash
  docker stop <container ID>
  ```

  ## Exposing ports in a docker machine.
  To expose a port simply use the switch `-p` followed by the ports you wish to expose.   
  The syntax is as follows:
  ```bash
  Docker run -p <host-IP>:<host-ports>:<docker-ports>
  ```

  **Example:**
  This nginex container will be accessible through 127.0.0.1:55010 on our host.
  ```bash
  docker run --myNginx -p 127.0.0.1:55010:80 nginx
  ```
  

## Expose an interactive session from the container to the machine.
```bash
docker run -it <image> 
```


