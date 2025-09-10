# Lab Assignment 2

In this lab, each student team will complete several tasks in the _Packet Sniffing and Spoofing_ and _TCP/IP Attack_ lab modules.

## Recommended background

Basic knowledge of computer networking is recommended. To get the most out of this lab, you needto have experience in computer networking (e.g., TCP/IP, socket programming) and/or spend some time learning about it. Additionally, familiarity with Docker networking configurations is important, as the lab may involve setting up and troubleshooting network communication between Docker containers.

## Environment Setup

Please refer to the related information in Lab 1.

### Intel/AMD Machines x86-64

1. Install VirtualBox first, https://www.virtualbox.org/ if you do not have it already. (Note: VirtualBox is available for most consumer computers, If you have trouble with this step, we encourage you to find a solution by yourself)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/manuals/vm/seedvm-manual.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the pre-built VM image (for Ubuntu 20.04 VM 64 bits). You cannot work on it directly on your personal machine.
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.
5. For Packet Sniffing and Spoofing Lab, download the lab specific zip file (Labsetup.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/Sniffing_Spoofing/).
6. For TCP/IP Attack Lab, download the lab specific zip file (Labsetup.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/TCP_Attacks/). You can download it directly on the VM or download it on your host machine and transfer it to the VM using the shared folder feature of VMware Fusion.
7. Unzip the setup file and start your lab.

### Apple Silicon Machines ARM64

1. Install VMware Fusion first, https://blogs.vmware.com/teamfusion/2024/05/fusion-pro-now-available-free-for-personal-use.html if you do not have it already. (Note: VMware Fusion is available for Apple Silicon M chiip Macs, If you have trouble with this step, we encourage you to find a solution by yourself)
2. VM setup instructions (read very carefully): https://github.com/seed-labs/seed-labs/blob/master/lab-setup/apple-arm/seedvm-fusion.md
3. Go to [Lab Environment Setup page](https://seedsecuritylabs.org/labsetup.html) to install the pre-built VM image (for Ubuntu 22.04 VM 64 bits). You cannot work on it directly on your personal machine.
4. After building the VM, you can start the VM and log in with the username and password provided in the lab setup page.
5. For Packet Sniffing and Spoofing Lab, download the lab specific zip file (Labsetup-arm.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/Sniffing_Spoofing/).
6. For TCP/IP Attack Lab, download the lab specific zip file (Labsetup-arm.zip) from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/TCP_Attacks/). You can download it directly on the VM or download it on your host machine and transfer it to the VM using the shared folder feature of VMware Fusion.
7. Unzip the setup file and start your lab.

## 1. Packet Sniffing and Spoofing (35 points)

https://seedsecuritylabs.org/Labs_20.04/Files/Sniffing_Spoofing/Sniffing_Spoofing.pdf

You only need to complete **Lab Task Set 1**, which includes four tasks: (1) Sniffing Packets, (2) Spoofing ICMP Packets, (3) Traceroute, and (4) Sniffing and then Spoofing.

**Sample code can be found here** (from the SEED Lab's creator): https://github.com/kevin-w-du/BookCode/tree/master/Sniffing_Spoofing

**Note:** When running the code for Task 1.3, please use your home network, as the school's network has security measures that may prevent the code from running successfully.

**Additional Question:** In 3.3 Task 1.3: Traceroute, we increment the TTL value to get the number of routers flowing through. Please explain why we can make this. (Hint: Getting to know what TTL is and the process of routing.)

## 2. TCP/IP Attack (15 points)

https://seedsecuritylabs.org/Labs_20.04/Files/TCP_Attacks/TCP_Attacks.pdf

You only need to complete Task1: SYNFlooding Attack (task 1.1 to task 1.3): **SYN Flooding Attack**.

**Additional Question:** Please explain how the SYN cookie mechanism can help to defend the SYN flood
attacks.

## Submission Details

- Each group only needs to submit one report in PDF format.
- Please list group members in your report explicitly.
- Only typed reports are accepted.
- Include screenshots with explanations in your report where applicable, to support your findings or steps taken.

## Grading

- Completeness (30 points): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
- Presentation (20 points): The report must be clear and correct in organization and writing with adequate explanation.
