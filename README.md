# 🖥️ OSX4VM - Run macOS Easily on Windows

[![Download OSX4VM](https://img.shields.io/badge/Download-OSX4VM-blue?style=for-the-badge)](https://github.com/FranckDJOUKWE/OSX4VM/releases)

---

## 📋 About OSX4VM

OSX4VM is a simple tool to run macOS on your Windows PC using WSL2. It sets up a virtual machine with macOS Tahoe. The setup uses OpenCore and QEMU/KVM for virtualization. This means you can run macOS without owning a Mac device.

This setup is designed to work smoothly on Windows or Linux. It uses an optimized kernel and a smart boot engine to make the experience stable and fast. You don’t need deep technical knowledge to get it running.

---

## 🖥️ System Requirements

Before you download and install, make sure your PC meets these basic requirements:

- **Operating System:** Windows 10 or later with WSL2 installed  
- **Processor:** Intel or AMD CPU with virtualization support (VT-x or AMD-V) enabled in BIOS  
- **RAM:** Minimum 8 GB; 16 GB or more recommended for better performance  
- **Disk Space:** At least 50 GB free space for macOS and virtual machine files  
- **Storage:** SSD preferred for faster boot and smooth use  
- **Other:** Internet connection to download files and necessary updates

---

## 🔧 What You Get with OSX4VM

- A clean and tested configuration for macOS Tahoe  
- OpenCore bootloader integrated for smooth macOS startup  
- QEMU/KVM virtualization for efficient performance on Windows and Linux  
- An optimized Linux kernel tailored for virtualization  
- Simple setup steps to bring macOS to your PC  
- Support for WSL2 to run macOS directly on Windows without dual boot

---

## 🚀 Getting Started

This section guides you step-by-step on how to download, install, and start OSX4VM on your Windows PC.

---

## ⬇️ Download OSX4VM

Visit the release page below to download the latest version of OSX4VM. The page contains all the necessary files and instructions for installation.

[Download OSX4VM from GitHub Releases](https://github.com/FranckDJOUKWE/OSX4VM/releases)

---

## 🛠️ Installation Steps

Follow these instructions carefully. Take your time to ensure each step is completed.

### 1. Enable WSL2 and Virtualization on Windows

- Press `Win + X` and select **Windows Terminal (Admin)** or **PowerShell (Admin)**  
- Run the command to enable WSL:

  ```
  wsl --install
  ```

- Restart your PC when prompted  
- Make sure virtualization is enabled in your PC BIOS. Look for VT-x or AMD-V setting and turn it on. Refer to your motherboard or PC manual if you need help.

### 2. Install a Linux Distribution for WSL2

- Open Microsoft Store and search for **Ubuntu** or your preferred Linux distro  
- Click **Get** and install it  
- After installation, launch the Linux app from the Start menu and create a user account  

### 3. Download OSX4VM Files

- Go to the [OSX4VM Release page](https://github.com/FranckDJOUKWE/OSX4VM/releases)  
- Download the latest release package (usually a ZIP file or similar)  
- Save it to an easy-to-find folder on your PC

### 4. Extract and Prepare Files

- Right-click the downloaded package and select **Extract All**  
- Move the extracted files into your Linux home folder.  
  You can do this by opening the Linux terminal and typing:  

  ```
  mv /mnt/c/path/to/downloaded/folder ~/
  ```

  Replace `/mnt/c/path/to/downloaded/folder` with the actual Windows path to your downloaded files.

### 5. Run the Setup Script

- In the Linux terminal, navigate to the extracted folder:

  ```
  cd ~/OSX4VM
  ```

- Run the setup script

  ```
  sudo ./setup.sh
  ```

  This script will install all the required dependencies and configure the virtual machine environment. You may be asked for your password.

### 6. Start macOS Virtual Machine

- After setup finishes, you can start the VM by running:

  ```
  ./start.sh
  ```

- The macOS Ventura installer or system should load inside the virtual machine window

---

## 🔍 What to Expect After Setup

- The VM window shows the macOS boot process  
- Installing macOS may take some time, especially if running for the first time  
- Follow the macOS on-screen instructions to complete installation  
- Once installed, you can use macOS like a regular Mac  
- The VM has internet access, shared files, and basic hardware support

---

## ⚙️ Troubleshooting Tips

- Make sure WSL2 is running and updated (`wsl --update`)  
- Restart your PC if virtualization doesn’t seem enabled  
- Check BIOS settings for VT-x or AMD-V options  
- If the VM fails to start, run `dmesg` in Linux to see kernel messages  
- Review the GitHub Issues page for common problems and fixes  
- Use a PC with an SSD for better performance

---

## 📚 Additional Resources

- [Official WSL2 Documentation](https://docs.microsoft.com/en-us/windows/wsl/)  
- [QEMU and KVM official documentation](https://www.qemu.org/documentation/)  
- [OpenCore Bootloader Guide](https://dortania.github.io/OpenCore-Install-Guide/)  

---

## 🔗 Download Link Reminder

Make sure to visit the GitHub releases page here:

[Download OSX4VM](https://github.com/FranckDJOUKWE/OSX4VM/releases)

Download the latest files and keep them updated for the best experience.