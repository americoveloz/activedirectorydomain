# Active Directory Windows Domain Implementation

### Introduction
This project demonstrates the deployment of an Active Directory Domain Services (AD DS) environment. Implementing a domain is a critical security baseline for organizations, enabling centralized management, identity verification, and the enforcement of security policies (GPOs) across all network endpoints.

### Lab network diagram
<img width="667" height="358" alt="Topology" src="https://github.com/user-attachments/assets/8399bc4c-7f3a-4bcb-99e9-a245647df6be" />


### Tools used
- VMware Workstation 25H2
- Windows Server 2022
- Windows 10 64bit


### Step-by-step Implementation

[Step 1 & 2 video](https://youtu.be/pctVqHIzsWo)

#### Step 1. Installed Windows Server on a Virtual Machine
<img width="1406" height="834" alt="image" src="https://github.com/user-attachments/assets/0d55c596-c5cd-4a83-812c-a9b2d78a3456" />
<i>Installation of Windows Server done</i>

#### Step 2. Enabled Active Directory Domain Services Role in Windows Server
Prerequisites:
- Set a static IP address to the server. Set the DNS server IP to point to itself using the same server's IP or 127.0.0.1.
- Configure a name to the server.

<img width="621" height="371" alt="image" src="https://github.com/user-attachments/assets/ac90895e-0b7f-4484-8aff-90965362151d" />
<i>Static IP and Named configured</i>

<img width="816" height="604" alt="image" src="https://github.com/user-attachments/assets/c059d788-4d3d-4f40-93c7-7592101a3169" />
<i>Enabling Active Directory Domain Services Role</i>

#### Step 3. Promoted the Server to Domain Controller
Note: It is important to use .local or a non-routable internal subdomain instead of .com. This prevents DNS conflicts between internal resources and public-facing websites.

<img width="857" height="677" alt="image" src="https://github.com/user-attachments/assets/1f2085c0-e086-46b4-8171-fce69ef50243" />
<i>Setting the domain name</i>

<img width="1134" height="408" alt="image" src="https://github.com/user-attachments/assets/0ef929a5-7723-418b-8a47-299fb9bb4491" />
<i>Server promoted to Domain Controller</i>


#### Step 4. Added Windows 10 VM to the Domain
Prerequisites:
- Set the dns server to the server's IP.
<img width="450" height="515" alt="image" src="https://github.com/user-attachments/assets/f8e37ff5-8b0b-4e82-84ac-ff532bc87e74" />
<i>DNS server setting in the Windows 10 VM</i>

Installation of Windows 10 on the VM [Video](https://youtu.be/6ZiSBbfSKsM)
Adding Windows 10 to the domain [Video](https://youtu.be/Jh-48SJ8rt0)

<img width="786" height="628" alt="image" src="https://github.com/user-attachments/assets/4f78d799-505c-4c4e-ba98-9fab85baa7fe" />
<i>Windows 10 VM properties showing it has been added to the domain<i>


### Outcome/Lessons Learned
With a Domain configured, a business can protect their devices, including servers and endpoints, from malicious ones trying to connect to the internal network. By implementing a Windows Domain, I established a centralized authentication authority. This project highlights the importance of identity as a security perimeter, ensuring that only authorized devices and users can access corporate resources. Key takeaways include DNS configuration, static IP management, and the fundamentals of domain join procedures.


### Other resources
- Download Windows 10 iso [Link](https://www.microsoft.com/en-us/software-download/windows10) [Video](https://youtu.be/yGYg5e4MKxg)
- Download Windows Server iso [Link](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2025)
- Download and installation of VMware Workstation from broadcom.com [Link](https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware%20Workstation%20Pro&freeDownloads=true) [Video](https://youtu.be/dAUnyVpmuwk)

