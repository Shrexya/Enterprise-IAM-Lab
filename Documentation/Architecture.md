# Enterprise Identity & Access Management (IAM) Lab

## 1. Project Overview

This project aims to build a simulated enterprise Identity and Access Management environment using Microsoft Active Directory.

The lab will demonstrate employee identity management, role-based access control, least privilege, account lifecycle management, and access auditing.

## 2. Proposed Lab Architecture

### Host System
- Operating System: Windows 11 Home
- Virtualisation: Oracle VirtualBox 7.2.22
- Administration Tools: PowerShell, VS Code, Git

### Virtual Machine
- VM Name: IAM-DC01
- Operating System: Windows Server 2025 Evaluation
- Edition: Standard Evaluation (Desktop Experience)
- RAM: 6 GB (planned)
- Virtual Processors: 2 (planned)
- Virtual Disk: 80 GB, dynamically allocated (planned)

### Active Directory Configuration
- Proposed Domain: ad.cybertech.test
- Domain Controller: IAM-DC01
- Directory Service: Active Directory Domain Services
- DNS: Active Directory-integrated DNS

## 3. Simulated Organisation

Company Name: CyberTech Solutions

Planned Departments:
- Information Technology
- Human Resources
- Finance
- Information Security

The environment will use fictional employee accounts and organisational units.

## 4. Planned Security Implementation

- Active Directory user and group management
- Role-Based Access Control (RBAC)
- Least Privilege Principle
- NTFS folder permissions
- Employee onboarding and offboarding
- Unauthorised access testing
- Access reviews and auditing
- PowerShell automation

## 5. Network Design

The initial lab will use an isolated VirtualBox Internal Network.

The domain controller will provide Active Directory and DNS services to the lab environment.

Additional client machines may be introduced later if system resources permit.

## 6. Tools and Technologies

- Windows Server 2025
- Active Directory Domain Services
- PowerShell
- Python
- Oracle VirtualBox
- Visual Studio Code
- Git and GitHub

## 7. Security Scope

All activities will be performed within an authorised local virtual environment.

Only fictional identities, test accounts, and test resources will be used.

No production systems or real employee accounts will be accessed.

## 8. Implementation Status

This document describes the proposed architecture.

The Windows Server virtual machine, Active Directory domain, DNS configuration, users, groups, and permissions have not yet been implemented or verified.

Implementation details will be updated as the lab progresses.
