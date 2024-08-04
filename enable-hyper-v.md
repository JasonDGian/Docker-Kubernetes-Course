# Enable Hyper-V on Windows 10 & Windows 11.
This guide will show you how to check if your machine is Hyper-V compatible, and if so, how to enable it.
 
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



