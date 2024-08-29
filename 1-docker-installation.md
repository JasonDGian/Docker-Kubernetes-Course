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
The Linux operating system natively supports containers and the associated technology.
In linux, though, an important distinction must be made between **Docker Engine** and **Docker Desktop**.
Docker engine 


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












