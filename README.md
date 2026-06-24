# active-directory-home-lab
Windows Server 2019 Active Directory home lab with DHCP, DNS, NAT, PowerShell user creation, and Windows 10 domain joining.

## Overview
This project documents the setup of a basic Active Directory home lab using Windows Server 2019 and Windows 10 in Oracle VirtualBox. The goal of this lab was to build a small enterprise-style Windows domain environment, configure core networking services, create domain users, and join a client machine to the domain.

This lab was completed by following a guided tutorial and documenting each step of the configuration process.

## Lab Environment
- Oracle VirtualBox
- Windows Server 2019
- Windows 10
- Active Directory Domain Services
- DNS
- DHCP
- NAT / Routing and Remote Access
- PowerShell

## What I Built
I created a virtualized domain environment with one Windows Server 2019 machine acting as the Domain Controller and one Windows 10 machine acting as the client. The server was configured with two network adapters: one for internet access and one for the internal lab network.

## Steps Completed
- Installed and configured a Windows Server 2019 virtual machine
- Configured internal networking for the lab environment
- Installed Active Directory Domain Services
- Promoted the server to a Domain Controller
- Created a new Active Directory forest named `mydomain.com`
- Configured Routing and Remote Access with NAT
- Installed and configured DHCP with an address scope of `172.16.0.100–172.16.0.200`
- Created a custom Domain Admin account
- Used PowerShell to generate over 1,000 Active Directory user accounts
- Created and configured a Windows 10 client virtual machine
- Verified network connectivity by pinging the domain
- Joined the Windows 10 client to the domain
- Confirmed the client appeared inside Active Directory Users and Computers
- Successfully logged into the Windows 10 client using a domain user account

## Key Skills Practiced
- Active Directory administration
- Windows Server configuration
- Domain Controller setup
- DHCP and DNS configuration
- NAT and internal network routing
- PowerShell scripting
- Virtual machine setup and troubleshooting
- Windows domain authentication
- Client-to-domain joining

## What I Learned
This lab helped me understand how Active Directory is used in real-world enterprise environments to manage users, computers, and authentication. I also gained hands-on experience with Windows Server roles, internal networking, DHCP scopes, domain joining, and basic PowerShell automation.

## Future Improvements
- Add Group Policy Objects
- Configure password and account lockout policies
- Create organizational units for different departments
- Add shared folders and permissions
- Connect the lab to a SIEM for event monitoring
- Practice detecting failed login attempts and account activity
