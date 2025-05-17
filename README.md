# Ex.3(A-C) Virtualization: Installation and Configuration of Oracle VirtualBox & Kali Linux, and Execution of Linux Commands
### NAME: DHINESH R
### REG NO:212223220019

## Aim:
To set up a virtualized environment using Oracle VirtualBox, install Kali Linux as a guest OS, and execute fundamental Linux commands.

## 3.a) Installation and Configuration of Oracle VirtualBox

## Aim:
To install and configure Oracle VM VirtualBox.

## Pre-requisites:

* Machine with Internet access
* Minimum 4 GB RAM
* Sufficient storage space

## Steps:
1. Download Oracle VM VirtualBox:

    * Visit Oracle VirtualBox Official Site
    * Download installer for your OS (Windows/macOS/Linux).
2. Install Oracle VM VirtualBox (Example: Windows):

    * Launch Installer → Allow Changes → Click Next.
    * Choose Installation Options → Click Next.
    * Accept Network Interface Warning → Click Yes.
    * Click Install.
    * Finish Installation and Launch VirtualBox.
3. Configure VirtualBox:

    * Open VirtualBox.
    * Click New → Name VM → Select Type (Linux/Windows) and Version.
    * Allocate:
        * Minimum 2 GB RAM
        * Create Virtual Hard Disk (20 GB recommended).
    * Start Virtual Machine and provide ISO to install OS.

## Result:
Thus, Oracle VM VirtualBox was installed successfully.

## 3.b) Installation and Configuration of Kali Linux

## Aim:
To install and configure Kali Linux in Oracle VirtualBox.

## Pre-requisites:
* Oracle VM VirtualBox Installed
* 4 GB RAM and 20 GB Storage Minimum
* Kali Linux ISO image

## Steps:
1. Download Kali Linux ISO:

    * Visit Kali Linux Official Site
    * Download 64-bit ISO (Installer version).
2. Create a New Virtual Machine:

    * Open VirtualBox → Click New.
    * Name: "Kali Linux" → Type: Linux → Version: Debian (64-bit).
3. Allocate Memory:

    * Minimum 2 GB RAM (recommended 4 GB).
4. Create Virtual Hard Disk:

    * Select VDI (VirtualBox Disk Image).
    * Choose Dynamically allocated.
    * Set Disk size to 20 GB or more.
5. Configure ISO Image:

    * Settings → Storage → Controller: IDE → Empty CD → Choose Disk File → Select Kali Linux ISO.
6. Start Installation:

    * Boot Virtual Machine → Choose Graphical Install.
    * Set Language, Region, Keyboard.
    * Configure Network → Set Hostname (e.g., kali).
    * Set root password.
    * Disk Partitioning: Use entire disk → All files in one partition.
    * Install System → Install GRUB Bootloader → Finish Installation.
7. Login to Kali Linux:

    * Use root credentials.
8. (Optional) Install Guest Additions:

    * Devices → Insert Guest Additions CD Image → Follow steps inside Kali.

## Snapshots:
AWS Account Creation Snapshot

Snapshot 1: Installing Oracle VirtualBox
![image](https://github.com/user-attachments/assets/737dafde-fd5d-4266-849a-a12013ce9c5b)

Snapshot 2: Kali Running in Virtual
![image](https://github.com/user-attachments/assets/6b08c65e-e2c0-4f8e-a782-0914a3470759)

## Result:
Thus, Kali Linux guest OS was installed and configured successfully.

## 3.c) Execution of Linux Commands in Kali

## About Linux:
* Open-source operating system.
* Kernel manages communication between hardware and software.
* Commands are case-sensitive.

## Linux Commands:
1. ls Command
    
    The ls command is used to display a list of content of a directory.

### Syntax:
```
ls
```
![image](https://github.com/user-attachments/assets/65cbb685-53e1-4d50-b109-2d3a73e366dc)

2. pwd Command

    The pwd command is used to display the location of the current working directory.

### Syntax: 
```
pwd
```
![image](https://github.com/user-attachments/assets/06a87e8c-9f1f-4f33-9c75-d9a5f75c8d60)


3. mkdir Command

    The mkdir command is used to create a new directory under any directory.

### Syntax: 
```
mkdir <directory_name>
```
![image](https://github.com/user-attachments/assets/1b1790eb-a58c-4bbb-a2b7-ee9ab6051a93)


4. rmdir Command

    The rmdir command is used to delete a directory.

### Syntax: 
```
rmdir <directory_name>
```
![image](https://github.com/user-attachments/assets/5002fe8b-4414-42d0-8519-3d1f452fbafb)


5. cd Command
The cd command is used to change the current directory

### Syntax: 
```
cd <directory_name>
```
![image](https://github.com/user-attachments/assets/84cead37-3512-4e54-8884-427cb99b15fc)


6. cat Command

    The cat command is a multi-purpose utility in the Linux system. It can be used to create a file, display content ofthe file, copy the content of one file to another file, and more.

### Syntax: 
```
cat [options] [file_name]
```
![image](https://github.com/user-attachments/assets/2361932b-99fc-4118-9097-bd9bdce384f0)

![image](https://github.com/user-attachments/assets/4c6d451f-4bfc-48f1-b4cd-0217fef9e06c)

7. cp Command

    The cp command is used to copy a file or directory.
### Syntax: 
```
cp [source] [destination]
```
![image](https://github.com/user-attachments/assets/4e377a91-23d4-4169-a66b-f88af203a60b)


![image](https://github.com/user-attachments/assets/1edbd41c-31c2-4a94-8e7f-be35155e35e5)


8. mv Command

    The mv command is used to move a file or a directory form one location to another location.

### Syntax: 
```
mv [source] [destination]
```
![image](https://github.com/user-attachments/assets/fd4832ba-1dad-45a7-a213-a5f28ca508db)


![image](https://github.com/user-attachments/assets/16138df9-da4a-4070-a936-29f251178773)


9. touch Command

    Create empty file.

### Syntax: 
```
touch [filename]
```
![image](https://github.com/user-attachments/assets/0ee05807-fe42-4579-a1bf-6562904fd7b1)


10. vi Command

    Edit file contents using editor.

### Syntax: 
```
vi [filename]
```
![image](https://github.com/user-attachments/assets/77ca13f3-45d7-4da6-88af-cdd2e280f41b)

## Result:
Thus, various Linux commands were executed successfully in Kali Linux virtual machine.
