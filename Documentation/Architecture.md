# Enterprise Identity & Access Management (IAM) Lab

## 1. Project Overview

This project implements a simulated enterprise Identity and Access Management environment using Microsoft Active Directory.

The lab demonstrates centralised identity management, departmental group-based access control, least privilege, employee account lifecycle management, and access auditing.

## 2. Lab Architecture

### Host System
- Operating System: Windows 11 Home
- Virtualisation: Oracle VirtualBox 7.2.22
- Administration Tools: PowerShell, VS Code, Git

### Domain Controller
- VM Name: IAM-DC01
- Operating System: Windows Server 2025 Evaluation
- Edition: Standard Evaluation (Desktop Experience)
- RAM: 6 GB
- Virtual Processors: 2
- Virtual Disk: 80 GB, dynamically allocated
- Static IPv4 Address: 192.168.50.10/24

### Active Directory Configuration
- Domain: ad.cybertech.test
- NetBIOS Name: AD
- Domain Controller: IAM-DC01
- Directory Service: Active Directory Domain Services
- DNS: Active Directory-integrated DNS
- Domain Controller Roles: DNS Server and Global Catalog

## 3. Simulated Organisation

**Company Name:** CyberTech Solutions

The Active Directory organisational structure contains the following departments:

- Information Technology (IT)
- Human Resources (HR)
- Finance
- Information Security

### Organisational Unit Structure

- CyberTech Solutions
  - IT
  - HR
  - Finance
  - Information Security

The departmental OUs are used to organise employee identities.

## 4. Identity and Group Management

### Provisioned Employee Accounts

| Employee | Department | Username |
|---|---|---|
| Rahul Sharma | IT | rahul.sharma |
| Priya Das | HR | priya.das |
| Arjun Roy | Finance | arjun.roy |
| Neha Sen | Information Security | neha.sen |

### Departmental Security Groups

| Security Group | Department |
|---|---|
| GG_IT | IT |
| GG_HR | HR |
| GG_Finance | Finance |
| GG_InfoSec | Information Security |

All four groups are configured as Global Security Groups. Each employee has been assigned to the corresponding departmental group.

## 5. Network Design

- Network Type: VirtualBox Internal Network
- Network Name: IAM-Internal
- Domain Controller IP: 192.168.50.10
- Subnet: 192.168.50.0/24
- Default Gateway: Not configured

The isolated network provides a controlled environment for Active Directory and DNS operations without exposing the lab domain to an external network.

A Windows client machine may be introduced later for domain authentication and access-control testing.

## 6. Planned Security Implementation

The following controls and activities remain part of the implementation roadmap:

- Role-Based Access Control (RBAC)
- Least Privilege Principle
- Department-specific shared folders
- NTFS and share permission management
- Employee onboarding and offboarding
- Department transfer and access revocation
- Unauthorised access testing
- Group Policy security configuration
- Access reviews and security auditing
- PowerShell automation

## 7. Tools and Technologies

- Windows Server 2025
- Active Directory Domain Services
- DNS Server
- PowerShell
- Python
- Oracle VirtualBox
- Visual Studio Code
- Git and GitHub

## 8. Security Scope

All activities are performed within an authorised local virtual environment.

Only fictional identities, test accounts, and test resources are used.

No production systems or real employee accounts are accessed.

## 9. Implementation Status

### Implemented
- Windows Server domain controller deployment
- Active Directory and DNS configuration
- Domain creation: ad.cybertech.test
- Departmental organisational units
- Employee account provisioning
- Departmental Global Security Groups
- Employee group membership assignment

### Pending
- Shared resource configuration
- NTFS and share permission enforcement
- Domain client authentication testing
- Group Policy configuration
- Identity lifecycle management
- Security auditing and access reviews
- PowerShell automation
- Final security validation and reporting

This document will be updated as additional components are implemented and tested.