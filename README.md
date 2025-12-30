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

### Step 1: Power on the server and connect the display in order to see the loading screen

screenshot

### Step 2: Looking at the loading screen press the F10 Key to enter the System Settings

screenshot

screenshot

### Step 3: Download Proxmox onto a USB (Stable version)

### Step 4: Update network settings to connect to Proxmox UI

delete ISOs
create snapshots
### Step 5: 

## Installing Proxmox

## Installing pfSense

## Installing Ubuntu

## Installing VPN 




