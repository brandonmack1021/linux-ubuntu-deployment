# Ubuntu Installation Steps

## 1. Download Ubuntu ISO
- Go to ubuntu.com/download
- Download the latest LTS version

## 2. Create Bootable USB
- Use Rufus
- Select USB device and Ubuntu ISO
- Set Partition Scheme: GPT
- Target system: UEFI
- File system: FAT32
- Start process

## 3. BIOS / UEFI Setup
- Enable USB boot
- Disable Secure Boot
- Set USB as first boot device

## 4. Install Ubuntu
- Boot from USB
- Select Install Ubuntu
- Choose Normal installation and enable updates
- Create primary user account

## 5. Post-install Update
```bash
sudo apt update && sudo apt upgrade -y

