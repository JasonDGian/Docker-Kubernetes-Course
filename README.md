# 📍 Index.
- [What is docker](README.md#what-is-docker)     
   - What is a container.  
   - Why use containers.   
   - Containers vs Virtual Machines.   
- [Docker installation](1-docker-installation.md)    
   - What is a docker container.   
   - What is a docker image.   
   - Container vs Image.   
- [Enabling hper V on windows](1.1-enable-hyper-v.md)    
   - Checking compatibility.  
   - Enabling Hyper-V on Win11.  
- [Images vs containers](2-images-and-containers.md)   


---

>[!WARNING]
> These notes are my personal writings taken during my Udemy Docker & Kubernetes Course - paid version. Feel free to use these notes but beware some concepts may be obsolete by the time you read this or perhaps entirely wrong.  

# 📌 What is Docker?
Docker is a technology that simplifies the creation and management of software development _containers_. 
   
## 🔹 What is a _container_?
A container in software development is a **standardized unit of software**. This unit packages code and all its necessary dependencies to run correctly. This allows developers to distribute and run 'ready to use' applications and server-like utilities.
   
> [!NOTE] 
> Support for Containers is built into modern operating systems and is a _must know_ tech for any aspiring developer.
      
## 🔹 Why use containers?
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

## 🔹 Docker containers VS Virtual Machines.
Docker containers provides similar functionality to conventional virtual machines, but there are key differences in their weight and computational cost. Docker containers are lighter and more efficient than virtual machines, which makes them faster to start and less resource-intensive. 
- Easy of use.
- Reduced set up time.
- Reduced weight and computational cost.

### ▫️ Virtual machines in comparison with Docker containers.
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

