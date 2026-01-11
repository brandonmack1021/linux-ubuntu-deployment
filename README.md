# Linux Operating System Deployment & System Configuration (Ubuntu)

## Project Overview
This project documents the deployment and configuration of Ubuntu Linux on a personal laptop.  
The goal is to demonstrate practical Linux system administration skills, including installation, system setup, and basic system updates.

---

## Environment
- **Operating System:** Ubuntu LTS (latest stable version)  
- **Hardware:** Laptop (bare-metal installation)  
- **Installation Method:** Bootable USB  
- **Tools:** Rufus (to create bootable USB), Bash, Git

---

## Objectives
- Install Ubuntu Linux from scratch  
- Configure the system and user account  
- Apply system updates and basic configuration  
- Document the installation process

---

## Step-by-Step Installation Guide

### 1. Download Ubuntu ISO
- Go to [ubuntu.com/download](https://ubuntu.com/download/desktop)  
- Download the latest **Ubuntu LTS** ISO file  

### 2. Create Bootable USB with Rufus
- Download **Rufus** from [rufus.ie](https://rufus.ie/)  
- Insert a USB flash drive (8 GB minimum)  
- Open Rufus and select:
  - **Device:** USB drive  
  - **Boot selection:** Ubuntu ISO  
  - **Partition scheme:** GPT  
  - **Target system:** UEFI  
  - **File system:** FAT32  
- Click **Start** and wait for it to finish  

### 3. BIOS / UEFI Setup
- Restart your laptop and enter BIOS/UEFI settings  
- Enable USB boot  
- Disable Secure Boot if needed  
- Set USB drive as the first boot device  

### 4. Install Ubuntu
- Boot from the USB drive  
- Select **Install Ubuntu**  
- Choose language and keyboard layout  
- Select **Normal installation**  
- Enable updates during installation  
- Create your primary user account  
- Let the installation complete  

### 5. First Boot & System Update
- Boot into Ubuntu desktop  
- Open Terminal and run:

```bash
sudo apt update && sudo apt upgrade -y
