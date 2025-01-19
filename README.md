# Win-Server-2022-RMIT-Cybersecurity-Project
One of my Blue teaming labs from my [RMIT Cybersecurity Project](https://github.com/Kazu010101/RMIT-Cybersecurity-Project/blob/main/README.md)

## Objective

- Install Windows Server 2022 on Oracle VirtualBox

## Lab Setup
- Oracle VirtualBox Installed
- Windows Server 2022 ISO File
- NAT Network Setting on Oracle VirtualBox

## Step 1: Mount Windows Server ISO Image on Oracle VirtualBox
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

*Figure 4: After the ISO image mounted, clicking Start icon powers up the VM for the installation process.*

## Step 2: Install Windows Server VM

- From the main installation windows:
1. Choose the language, and time & currency format, and click on Next
2. Click on Install now
3. For GUI installation, select 'Windows Server 2022 Datacenter Evaluation (Desktop Experience), and click on Next
4. Accept the license agreement and Click on Next

![wininstall](https://github.com/user-attachments/assets/fc2e485b-20a8-4a08-90dc-29adbb57c57a)

*Figure 5: On step 3, selecting other options beside (Desktop Experience) will install using CLI.*

5. Choose the installation as Custom
6. Choose the hard disk defined earlier, and click on Next
7. The windows server installation will now begin; this will take some time to finish
8. Setup the admin password, and click Finish

![wininstalfin](https://github.com/user-attachments/assets/67adee3b-63f3-4614-b050-56b09914ebb3)

*Figure 6: After step 8, installation of Windows server 2022 in Oracle VirtualBox is completed and we can log in into the Windows Server.*

It is also recommended to install the VirtualBox guest addition, which will improve the performance of the Windows Server VM.

## Result

The Windows Server 2022 VM is installed. We can improve the performance by installing the VirtualBox guest addition. 

The next important process in the project is to install Active Directory on Windows Server to have a centralized control over employees accounts. 

