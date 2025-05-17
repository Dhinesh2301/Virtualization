# Ex.3(A-C): Virtualization - Oracle VirtualBox & Kali Linux Setup

## Aim

This focuses on setting up a virtualized environment using Oracle VirtualBox, followed by the installation of Kali Linux as a guest operating system. It also covers the execution of fundamental Linux commands, enabling learners to interact with the system via the command line interface.

---

## Procedure

### A) Installation and Configuration of Oracle VirtualBox

#### Aim
To install and configure Oracle VM VirtualBox on your system.

#### Pre-requisites
- A machine with internet connectivity.
- Minimum 4 GB RAM (recommended for running virtual machines smoothly).
- Sufficient storage space (at least 20 GB) to host virtual machines.

#### Steps

1. **Download Oracle VM VirtualBox**  
   - Navigate to the official website: [https://www.virtualbox.org](https://www.virtualbox.org)  
   - Click **Download VirtualBox**.  
   - Select the installer for your operating system:
     - **Windows** → Windows Hosts
     - **macOS** → OS X Hosts
     - **Linux** → Choose your distro (Debian, Ubuntu, Fedora, etc.)

2. **Install Oracle VM VirtualBox (Windows Example)**
   - **Step 1:** Launch Installer and allow changes to the device.
   - **Step 2:** The Setup Wizard appears → Click **Next**.
   - **Step 3:** Choose default installation options.
   - **Step 4:** Accept network interface warning → Click **Yes**.
   - **Step 5:** Click **Install** and wait for it to complete.
   - **Step 6:** Click **Finish** and optionally launch VirtualBox.

3. **Configure VirtualBox**
   - Launch Oracle VM VirtualBox.
   - Click **New** to create a virtual machine.
   - Enter:
     - Name: Any name (e.g., Kali Linux)
     - Type: Linux
     - Version: Debian (64-bit)
   - Allocate resources:
     - RAM: At least 2 GB (2048 MB)
     - Hard Disk: Create a virtual hard disk (20 GB recommended)
   - After creating the VM, insert your OS ISO to install.

#### Result
Oracle VM VirtualBox was successfully installed and configured.

---

### B) Installation and Configuration of Kali Linux

#### Aim
To install and configure Kali Linux in Oracle VM VirtualBox.

#### Pre-requisites
- Oracle VM VirtualBox installed
- 4 GB RAM and 20 GB free disk space
- Kali Linux ISO image: [https://www.kali.org/get-kali/](https://www.kali.org/get-kali/)

#### Steps

1. **Download Kali Linux ISO**
   - Visit the official Kali Linux download page.
   - Choose **Installer** version (64-bit recommended).
   - Download the `.iso` file.

2. **Create a New Virtual Machine**
   - Open VirtualBox → Click **New**.
   - Name: `Kali Linux`
   - Type: `Linux`, Version: `Debian (64-bit)`
   - RAM: Allocate **2 GB** or more
   - Create a virtual hard disk → VDI → Dynamically Allocated → 20 GB+

3. **Configure ISO for Boot**
   - Go to **Settings** → **Storage**.
   - Under **Controller: IDE**, click **Empty** → CD icon → Choose a disk file...
   - Select your Kali Linux ISO.
   - Click **OK**.

4. **Start the Virtual Machine**
   - Click **Start** to boot from ISO.
   - Choose **Graphical Install**.

5. **Kali Linux Installation Steps**
   - **Language, Location, Keyboard** → Set as preferred.
   - **Network** → Enter hostname (e.g., kali), leave domain blank.
   - **Users** → Set a root password.
   - **Partitioning** → Choose:
     - Guided - use entire disk
     - All files in one partition
   - **Install System** → Wait for setup to complete.
   - **GRUB Bootloader** → Install to virtual hard disk.
   - **Finish** → Reboot VM.

6. **Login**
   - Login using `root` and the password you set.

7. **(Optional) Install Guest Additions**
   - In VirtualBox menu → Devices → Insert Guest Additions CD Image.
   - Follow on-screen instructions inside Kali Linux.

---

### C) Execution of Essential Linux Commands

Once Kali Linux is installed and running, open the terminal and try these basic commands:

```bash
pwd             # Show current directory
ls              # List directory contents
cd <dir>        # Change directory
mkdir <name>    # Create a new directory
rm <file>       # Delete a file
cp <src> <dst>  # Copy a file
mv <src> <dst>  # Move or rename a file
cat <file>      # View file contents
clear           # Clear the terminal
ifconfig        # View network configuration
```
### Snapshots
![image](https://github.com/user-attachments/assets/df1a3a8e-d15a-4ebe-948a-f18e5d9289cb)
Snapshot 1: Installing Oracle VirtualBox 

![image](https://github.com/user-attachments/assets/1c088d72-53bd-40a8-91f7-865230fd60d4)
Snapshot 2: Adding Kali (Guest OS) on Oracle VirtualBox

![image](https://github.com/user-attachments/assets/acb499cf-4124-4429-a96d-00dde65bb561)
Snapshot 3 :  Kali - The guest OS on Oracle Virtualbox
