> [!IMPORTANT]
> Unlike other posts in my repos, this is a copy paste with a little bit of formatting from an official website of Microsoft Windows.   
> **If you wish to see the original post you can find it [here](https://techcommunity.microsoft.com/t5/educator-developer-blog/step-by-step-enabling-hyper-v-for-use-on-windows-11/ba-p/3745905) .**

# Enable Hyper-V on Windows 10 & Windows 11.
This guide will show you how to check if your machine is Hyper-V compatible, and if so, how to enable it.

---
 
## Step 1: Check if your system is compatible. 
Before you can enable Hyper-V on your Windows 11 machine, you need to make sure that your system is compatible. Here are the system requirements for Hyper-V on Windows 11:

>    - Windows 11 Pro or Enterprise 64-bit Operating System 
>    - A 64-bit processor with Second Level Address Translation (SLAT)
>    - A minimum of 4 GB of RAM
>    - BIOS-level hardware virtualization support

### Steps to check if your system is compatible:
1. Press the `Windows key` + `R` to open the **Run** dialog box.
2. Type `msinfo32` and press Enter.
3. In the **System Information window**, scroll down to the **System Summary** section and look for the **Hyper-V Requirements** line. If it says "_Yes_", then your system is compatible.

---

## Step 2: Enable Hyper-V on Windows 11
Once you have confirmed that your system is compatible, you can proceed to enable Hyper-V on your Windows 10/11 machine.   
Here's how:

1. Press the `Windows key` + `R` to open the **Run** dialog box.
2. Type `appwiz.cpl` and press Enter.
3. In the **Programs and Features** window, select **Turn Windows features on or off** in the left-hand pane.
       
![imagen](https://github.com/user-attachments/assets/bbcb685f-75e7-4e53-8b52-efc035ad8222)
   
5. In the Windows Features window, scroll down to **Hyper-V** and check the box next to it.
   
![imagen](https://github.com/user-attachments/assets/6e88e450-9ce3-4f82-93e3-b2bac1d99b96)

6. Click on `OK` and wait for the installation process to complete.
7. Once the installation is complete, click on `Restart Now` to restart your computer.

---

## Step 3: Configure Hyper-V settings
After enabling Hyper-V on your Windows 11 machine, you may want to configure some settings to optimize your virtual machine performance. Here are some settings you may want to consider:

- **Virtual switch:** Hyper-V uses a virtual switch to connect virtual machines to your physical network. You can create a new virtual switch or use an existing one.
 
- **Virtual machine settings:** You can configure various settings for your virtual machine, such as memory allocation, processor allocation, and network adapter settings.  
    
- **Integration services:** Hyper-V integration services enhance the performance and functionality of virtual machines. You can enable or disable integration services as needed.

  Further resources surrounding the enablement of these resources can be found here: [Hyper-V Resource Settings](https://learn.microsoft.com/es-es/training/modules/configure-manage-hyper-v/?WT.mc_id=academic-89565-abartolo)

---

# READ THIS
In the original post this was not mentioned, therefore I wrote it down here. 

After enabeling Hyper-V follow these steps to enable Containers on Windows. 
 1. Open PowerShell as administrator.
 2. Run the command `Enable-WindowsOptianlFeature -Online -FeatureName Microsoft-Hyper-V -All`
 3. Restart your machine.
 4. Run the command `Enable-WindowsOptianlFeature -Online -FeatureName containers -All`

> [!Note]
> If the terminal says something like "Command was not found" you are probably not running PowerShell as an administrator, try to close and re-open with administrator privileges.
