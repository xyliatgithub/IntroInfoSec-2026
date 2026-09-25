# Lab Assignment 2

In this lab, each student team will complete several tasks in the _Packet Sniffing and Spoofing_ and _TCP/IP Attack_ lab modules.

## Recommended background

Basic knowledge of computer networking is recommended. To get the most out of this lab, you need to have experience in computer networking (e.g., TCP/IP, socket programming) and/or spend some time learning about it. Additionally, familiarity with Docker networking configurations is important, as the lab may involve setting up and troubleshooting network communication between Docker containers.

## Environment Setup
> [!IMPORTANT]
> If your laptop runs into VM issues, you can always do the lab on the **MSSI Lab** computers. 

1. Please reuse the VM/environment from **Lab 1**. If you already finished Lab 1 setup, you can skip this section. Otherwise, follow: [Lab 1 – Environment Setup](../lab1/README.md#environment-setup).
2. For Packet Sniffing and Spoofing Lab, download the lab specific zip file **matching your CPU** from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/Sniffing_Spoofing/):
   
   - Intel/AMD (x86-64): `Labsetup.zip`
   - Apple Silicon (ARM64): `Labsetup-arm.zip`
    
3. For TCP/IP Attack Lab, download the lab specific zip file **matching your CPU** from the [lab page](https://seedsecuritylabs.org/Labs_20.04/Networking/TCP_Attacks/):

   - Intel/AMD (x86-64): `Labsetup.zip`
   - Apple Silicon (ARM64): `Labsetup-arm.zip`
    
4. You can download directly inside the VM, or download on your host and transfer it to the VM using the shared folder feature (VirtualBox/VMware Fusion). Unzip the file and start your lab.


## 1. Packet Sniffing and Spoofing (25 points)

https://seedsecuritylabs.org/Labs_20.04/Files/Sniffing_Spoofing/Sniffing_Spoofing.pdf

You only need to complete **Lab Task Set 1**, which includes four tasks: (1) Sniffing Packets, (2) Spoofing ICMP Packets, (3) Traceroute, and (4) Sniffing and then Spoofing.

**Sample code:**
1. Task Set 1 uses Python (Scapy); all needed code samples are already in the PDF (§3.1–§3.4), which are sufficient on its own.
2. The linked repo (https://github.com/kevin-w-du/BookCode/tree/master/Sniffing_Spoofing) is C code for Task Set 2 — optional reference only, not required here.

**Notes:**
1. **Task 1.3:** please use your home network as necessary — the school's network has security measures that may prevent the code from running successfully.
2. **Task 1.4:** no sample code is given. Write your own Scapy (Python) sniff-and-spoof for ICMP by combining Tasks 1.1 and 1.2 (the C code in the linked repo is for UDP and can't be used directly).
   *Hints:*
   - Use `sniff()` (as in Task 1.1) to capture ICMP echo requests, and inside the callback build a spoofed reply with `send()` (as in Task 1.2).
   - Filter for echo requests only, e.g. `filter='icmp and icmp[icmptype]=8'`.
   - In the spoofed reply: swap source/destination IP, set ICMP `type=0` (echo reply), and copy the request's `id`, `seq`, and payload — otherwise `ping` won't accept it.

**Additional Question:** In 3.3 Task 1.3: Traceroute, we increment the TTL value to get the number of routers flowing through. Please explain why we can make this. (Hint: Getting to know what TTL is and the process of routing.)

## 2. TCP/IP Attack (15 points)

https://seedsecuritylabs.org/Labs_20.04/Files/TCP_Attacks/TCP_Attacks.pdf

You only need to complete Task1: SYN Flooding Attack (task 1.1 to task 1.3): **SYN Flooding Attack**.

**Additional Question:** Please explain how the SYN cookie mechanism can help to defend the SYN flood
attacks.

## Submission Details

- Each group only needs to submit one report in PDF format.
- Please list group members in your report explicitly.
- Only typed reports are accepted.
- Include screenshots with explanations in your report where applicable, to support your findings or steps taken.

## Grading

- Completeness (25 points): All the steps as instructed in the lab manual must be included in the report with adequate evidence.
- Presentation (15 points): The report must be clear and correct in organization and writing with adequate explanation.
