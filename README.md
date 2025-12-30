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

![2.jpeg](/images/2.jpeg)

Select `System BIOS` and make sure Secure Boot is `Disabled`
![3.jpeg](/images/3.jpeg)

### Step 3:
![4.jpeg](/images/4.jpeg)
![5.jpeg](/images/5.jpeg)
![6.jpeg](/images/6.jpeg)
![7.jpeg](/images/7.jpeg)
![8.jpeg](/images/8.jpeg)
![9.jpeg](/images/9.jpeg)

Make sure to select `Physical Disks` and put in the HDD or SDD you wish to use. In my case I only have a single SDD. Name your virtual disk and default settings are fine so click `Create Virtual Disk`
### Step 3: Download Proxmox onto a USB (Stable version)

### Step 4: Update network settings to connect to Proxmox UI

delete ISOs
create snapshots
### Step 5: 

## Installing Proxmox

## Installing pfSense

## Installing Ubuntu

## Installing VPN 




