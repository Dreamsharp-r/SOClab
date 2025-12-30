# SOClab

## Purpose

Document the end-to-end process of bringing a server online, installing a hypervisor, configuring management access, adding in segmentation and security via a firewall, partitioning for windows and linux users and lastly adding in a SIEM. 

## Scope


## Network Diagram


## Hardware Overview

### Management Workstation

Macbook M2 Air

### Server

| Component    | Details                                |
| ------------ | -------------------------------------- |
| Server Model | Dell PowerEdge R630                    |
| CPU          | 48x Intel Xeon E5-2680 v3              |
| RAM          | 32 GB DDR4                             |
| Storage Model| PERC H730 Mini                         |
| Storage      | 799.54 GB SSD (RAID 0)                 |
| NICs         | Onboard NICs + iDRAC                   |
| Management   | iDRAC                                  |


### Removable Storage
USB

### Peripherals

mouse
keyboard
WiFi Repeater
Display
Thunderbolt to Ethernet + USB 

## Server Configuration

### Step 1: 
Power on the server and connect the display in order to see the loading screen
> [!NOTE]
> Ignore the warning about SD card slots as this is not required.
> You can disable this within the settings. 


![1.jpeg](/images/1.jpeg)

### Step 2:
Looking at the loading screen press the F2 Key to enter the System Settings
> [!NOTE]
> Ignore the IP address change. I had to go back and recreate the steps 
> To fully document this setup.

![2.jpeg](/images/2.jpeg)

Select `System BIOS` and make sure Secure Boot is `Disabled`
![3.jpeg](/images/3.jpeg)

![4.jpeg](/images/4.jpeg)

### Step 3:
Go back and click into `Integrated Devices`. Make sure Integrated RAID Controller is set to `Enabled`.
![5.jpeg](/images/5.jpeg)

### Step 4:
Go back and click into `SATA Settings`. Make sure Embedded SATA is set to `RAID MODE`
![6.jpeg](/images/6.jpeg)

### Step 5:
At this point exit the menu and save all changes. Once saved restart the server and log back into `System Setup`. Under `Device Settings` you should now see `Integrated RAID Controller 1` with your hard drive name after that. 
![7.jpeg](/images/7.jpeg)

### Step 7:
Click the drive and click `Configuration Management` then `Create Virtual Disk`. Make sure to select your physical disk and the disk size will automatically be set. Name the virtual drive and keep the default settings and click `Create Virtual Disk`
![8.jpeg](/images/8.jpeg)

![9.jpeg](/images/9.jpeg)

After configuring you’ll see the virtual disk ready to go. Exit and save everything. Restart the server and press F11 for the `Boot Manager`
![10.jpeg](/images/10.jpeg)

### Step 8:
Unfortunately I forgot to take a screenshot of this step. But its pretty easy. Just switch the boot order to boot from your Proxmox OS you already configured. After that reboot and you will find yourself at this screen. 
![11.jpeg](/images/11.jpeg)
### Step 3: Download Proxmox onto a USB (Stable version)

### Step 4: Update network settings to connect to Proxmox UI

delete ISOs
create snapshots
### Step 5: 

## Installing Proxmox

## Installing pfSense

## Installing Ubuntu

## Installing VPN 




