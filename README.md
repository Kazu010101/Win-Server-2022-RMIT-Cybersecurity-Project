# Win-Server-2022-RMIT-Cybersecurity-Project
One of my Blue teaming labs from my [RMIT Cybersecurity Project](https://github.com/Kazu010101/RMIT-Cybersecurity-Project/blob/main/README.md)

## Objective

- Install Windows Server 2022 on Oracle VirtualBox

## Lab Setup
- Oracle VirtualBox Installed
- Windows Server 2022 ISO File
- NAT Network Setting on Oracle VirtualBox

## VM Installation Steps
- Open VirtualBox and click on New or CTRL+N to start the Windows Server VM installation.
- On the new Create Virtual machine window, the fields are specified as follows:
![svr1](https://github.com/user-attachments/assets/8d513a44-309a-4f64-bcae-f7944bd3128a)

*Figure 1: Specifying the VM name, save folder, OS type and Version. After finished, click Next.*

- Specify 2 GB RAM and 2 CPU Processors > Next
- Specify 50 GB of Hard disk > Next
![Setup for VM](https://github.com/user-attachments/assets/901b7120-87a4-448a-aa0a-1d8ff2775a65)

*Figure 2: Summary of the Windows Server VM Setup*

- Attach the Windows Server ISO File to VirtualBox by following the steps as shown in the screenshot below:
1. Click the Windows Server just created
2. Click Setting 
3. Click Storage 
4. On storage Device, click 'Empty' 
5. Click the disk icon
6. Click 'Choose a disk file...'
7. Select the Win Server ISO file from the folder
8. Click Next
9. At the Storage setting interface, click OK

![isofin2](https://github.com/user-attachments/assets/d9b1bb06-d0a0-4d09-89be-6a05c19b7fb4)


*Figure 3: Steps to attach ISO image*

- Back to the VirtualBox main interface, with the Windows Server VM selected on the left pane, click the Start Icon and the Windows Server VM installation starts.

![isofin4](https://github.com/user-attachments/assets/2e0855a9-943a-4417-a52e-ca49e814b3c0)

*Figure 4: With the ISO image mounted, clicking start powers up the VM for the installation process.*

## Result

The most important information from the nmap scan is that there are 3 open TCP ports, which are 135, 139, and 445. Considering that the target also uses Windows 10 OS, these information suggest that the host is running a file sharing service such as SMB protocol, which can be further exploited by the attacker.

