# Ubuntu Installation Steps

## 1. Download Ubuntu ISO
- Go to [ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)
- Download the latest **Ubuntu LTS ISO** (AMD64)

## 2. Create Bootable USB with Rufus
- Download Rufus 64-bit from [rufus.ie](https://rufus.ie/)
- Insert USB drive (8 GB minimum)
- Open Rufus:
  - Device: select USB
  - Boot selection: select Ubuntu ISO
  - Partition scheme: GPT
  - Target system: UEFI
  - File system: FAT32/NTFS (Rufus handles automatically)
- Click **Start** → Wait until it says **Ready** → Click **Close**
- Safely eject USB

## 3. Boot from USB
- Turn off laptop
- Press **Novo button** or **F12/F2** during startup to enter Boot Menu
- Select USB drive → press Enter
- Select **Install Ubuntu** (or Try Ubuntu first if testing)

## 4. Installer Options
- **Installation type:** Interactive Installation
- **Apps selection:** Default selection
- **Install recommended proprietary software:** Check both boxes (graphics/Wi-Fi drivers + media codecs) or leave unchecked if you want a fully open-source setup
- **Disk setup:**
  - Single OS: choose **Erase disk and install Ubuntu**
  - Dual-boot: choose **Manual / Something Else**
- **Encryption & file system:** No encryption, EXT4 filesystem
- **Create account:**
  - Enter name, computer name, username, password
  - Check **Require my password to login**
  - Leave **Use Active Directory** unchecked
- **Time zone:** select your local time zone

## 5. Finish Installation
- Click **Install** and wait for the process to complete
- When finished, reboot system and remove USB

## 6. First Login & System Updates
- Log in to Ubuntu using the account created during installation.
- During first login, you may be prompted:
  - **“Help improve Ubuntu by sharing system data with the Ubuntu team”**
  - Select **“No, don’t share system data”**.

- Open the Terminal:
  - Press **Ctrl + Alt + T**
    **OR**
  - Click **Activities** (top-left) → search **“Terminal”** → open it.

- Update the system:
```bash
sudo apt update && sudo apt upgrade -y
```
