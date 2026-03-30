# Active Directory Windows Domain Implementation

## Introduction



## Lab network diagram
<img width="667" height="358" alt="Topology" src="https://github.com/user-attachments/assets/8399bc4c-7f3a-4bcb-99e9-a245647df6be" />


## Utilities & Tools used
- VMware Workstation 25H2
- Windows Server 2022
- Windows 10 64bit


## Step-by-step Implementation
### Step 1. Installed Windows Server on a Virtual Machine

### Step 2. Enabled Active Directory Domain Services Role in Windows Server
Prerequisites:
- Set a static IP address to the server. Set the dns server IP pointing to itself using the same server's IP or 127.0.0.1.
- Configure a name to the server.

### Step 3. Promoted the Server to Domain Controller

It is important to use .local at the end of the domain instead of .com. This is for the users in the internal network not to have problem surfing the website page with the same domain name.

### Step 4. Added Windows 10 VM to the Domain
Installation of Windows 10 on the VM [Video]
Prerequisites:
- Set the dns server to the server's IP.


## Outcome/Lessons Learned



## Other resources
- Download Windows 10 iso [Link] [Video]
- Download Windows Server iso [Link] [Video]
- Download and installation of VMware Workstation from broadcom.com [Link] [Video]

