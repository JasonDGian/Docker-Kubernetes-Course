# What is Docker?
Docker is a technology that simplifies the creation and management of software development _containers_. 
   
## What is a _container_?
A container in software development is a **standardized unit of software**. This unit packages code and all its necessary dependencies to run correctly. This allows developers to distribute and run 'ready to use' applications and server-like utilities.
   
> [!NOTE] 
> Support for Containers is built into modern operating systems and is a _must know_ tech for any aspiring developer.
      
## Why use containers?
When a software application requires a specific version of a dependency to run correctly, using containers helps the developer ensure that the application always uses the correct version of that dependency. 

> [!IMPORTANT]
> It is crucial to have the exact same environment for development and production. This consistency ensures that the application will work exactly as it was tested when deployed in a real-world setting.


**Key takeaways**
- Docker is a container management technology.
- Containers are standardized software units composed by [ `code` + `dependency` ].
- Using containers:
    - Eliminates dependency inconsistency problems and ensures the same environment for development and production .
    - Project dockerization: Lets developers distribute and run ready-to-use applications and server utilities.
    - Seamless version switch: Enables developers to use different dependency versions on the same machine without conflicts.

## Docker containers VS Virtual Machines.
Docker containers provides similar functionality to conventional virtual machines, but there are key differences in their weight and computational cost. Docker containers are lighter and more efficient than virtual machines, which makes them faster to start and less resource-intensive. 
- Easy of use.
- Reduced set up time.
- Reduced weight and computational cost.

### Virtual machines in comparison with Docker containers.
Comparing VMs with Docker we can argue the following pro and cons.
<table>
   <tr>
      <th>PRO</th>
      <th>CON</th>
   </tr>
   <tr>
      <td>Separated environments.</td>
      <td>Redundant duplication, waste of space.</td>
   </tr>
   <tr>
      <td>Environment-specific configurations are possible.</td>
      <td>Performance can be slow, boot times can be long.</td>
   </tr>
   <tr>
      <td>Environment configurations can be shared and reproduced reliably.</td>
      <td>Reproducing on another workstation/server is possible but may still be tricky</td>
   </tr>
</table>

<p align="center">
   <img height="320px" src="https://github.com/user-attachments/assets/a41d4fa7-cb89-49de-9610-6bf59c1209cc">
</p>
  
---

# Docker Installation
Docker can be installed on **macOS**, **Windows**, and **Linux**, with each operating system having specific requirements that must be met before installation.

## 🍎 MacOS & 🪟 Windows.
Depending on your device's specifications, you will need to install either **Docker Desktop** or **Docker Toolbox**:
    - **Docker Desktop**: This is the 'standard' version for devices that meet the system requirements.
    - **Docker Toolbox**: An alternative for devices that do not meet the requirements for Docker Desktop.

## 🐧 Linux
On Linux the operating system natively supports containers and the associated technology. For the installation follow the official resources.

- - - TODO - - -
    - SIMPLE GUIDE
- - - - - - - - 

---


### Windows installation.

### Check requirements.
   #### System requirements.
   #### Software requirements.
   
### Get the installer.
### Run the installer.

