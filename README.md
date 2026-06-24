# Active Directory Home Lab

![Windows Server](https://img.shields.io/badge/Windows_Server-2019-blue)
![Active Directory](https://img.shields.io/badge/Active_Directory-AD_DS-0078D4)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE)
![VirtualBox](https://img.shields.io/badge/Oracle-VirtualBox-2F61B4)
![Windows 10](https://img.shields.io/badge/Windows-10-0078D6)

---

## Overview

This project demonstrates the deployment of a small enterprise Active Directory environment using Windows Server 2019 and a Windows 10 client within Oracle VirtualBox. The lab focused on configuring a Domain Controller, Active Directory Domain Services (AD DS), DNS, DHCP, Routing and Remote Access (NAT), PowerShell automation, and client authentication within a Windows domain.

---

## Lab Architecture

The following diagram illustrates the completed lab environment.

<p align="center">
<img width="624" height="369" alt="image" src="https://github.com/user-attachments/assets/b4d8553e-bb76-4554-865a-d8d2769e0fd0" />
</p>

The environment consists of:

- Windows Server 2019 Domain Controller
- Windows 10 Client
- Oracle VirtualBox
- Internal Virtual Network
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Routing and Remote Access (NAT)

---

## Technologies Used

The following technologies were used throughout this project to deploy and configure the Active Directory environment.

- Windows Server 2019
- Windows 10
- Oracle VirtualBox
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Routing and Remote Access (NAT)
- PowerShell

---

## Project Walkthrough

### 1. Network Configuration

Configured the server's internal network adapter with a static IP address and DNS settings in preparation for promoting the server to a Domain Controller.

<p align="center">
<img width="452" height="517" alt="image" src="https://github.com/user-attachments/assets/16bf3c92-87e2-4682-86cc-800c2f5bc65f" />
</p>

---

### 2. Active Directory Deployment

Installed the **Active Directory Domain Services (AD DS)** server role and promoted the server to a **Domain Controller** by creating a new Active Directory forest named:

```text
mydomain.com
```

---

### 3. DHCP & Routing Configuration

Configured the **DHCP Server** role by creating an IPv4 address scope for client machines and enabled **Routing and Remote Access (NAT)** to provide network connectivity between the internal virtual network and the Internet.

---

### 4. PowerShell User Automation

Used a PowerShell script to automatically generate **1,000+ Active Directory user accounts**, demonstrating basic administrative automation and bulk user provisioning.

<p align="center">
<img width="613" height="809" alt="image" src="https://github.com/user-attachments/assets/d0de8d66-f433-40d8-a6d2-4da54ea668c5" />
<br><br>
<img width="344" height="421" alt="image" src="https://github.com/user-attachments/assets/0b84ecd4-5e6a-413f-8f64-bc7b13643161" />
</p>

---

### 5. Client Connectivity

Verified **DNS** resolution and communication between the **Windows 10 client** and the **Domain Controller** by successfully resolving and pinging the Active Directory domain.

<p align="center">
<img width="467" height="200" alt="image" src="https://github.com/user-attachments/assets/34bae2e3-9f4d-418b-86ff-4a748abe29d2" />
</p>

---

### 6. Joining the Domain

Configured the Windows 10 client to join the **mydomain.com** Active Directory domain.

<p align="center">
<img width="409" height="487" alt="image" src="https://github.com/user-attachments/assets/8598885d-b498-4131-a0d2-255576434e4c" />
</p>

---

### 7. Domain Verification

Confirmed that the Windows 10 client successfully appeared within **Active Directory Users and Computers**, verifying successful domain enrollment and authentication.

<p align="center">
<img width="619" height="430" alt="image" src="https://github.com/user-attachments/assets/a58ded79-b21a-4ddc-af0b-b4c9f3a9e0c1" />
</p>

---

## Skills Demonstrated

- Active Directory Administration
- Windows Server Administration
- Domain Controller Deployment
- Active Directory Domain Services (AD DS)
- DNS Configuration
- DHCP Configuration
- Routing and Remote Access (NAT)
- PowerShell Automation
- Windows Domain Authentication
- Client Domain Joining
- Enterprise Network Administration
- Oracle VirtualBox Virtualization

---

## What I Learned

This project provided hands-on experience deploying an enterprise Windows domain from the ground up. I gained practical experience configuring Active Directory, DNS, DHCP, Routing and Remote Access (NAT), and Windows authentication while learning how these services work together within an enterprise environment. Additionally, I developed familiarity with PowerShell automation for administrative tasks and the process of deploying, configuring, and managing virtual machines using Oracle VirtualBox.

---

## Future Improvements

Future enhancements to this lab include:

- Configure Group Policy Objects (GPOs)
- Implement password and account lockout policies
- Create Organizational Units (OUs) for department management
- Configure shared folders and NTFS permissions
- Deploy additional domain-joined client machines
- Configure Windows Event Forwarding
- Integrate Microsoft Sentinel for centralized log monitoring
- Expand the environment into a multi-server Active Directory lab
