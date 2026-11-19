# Enterprise Identity & Access Management (IAM) Lab

A hands-on enterprise IAM lab built using **Microsoft Active Directory** and **Windows Server 2025** to demonstrate centralised identity management, departmental access control, and security administration.

## Project Overview

This project simulates the IT identity infrastructure of a fictional organisation, **CyberTech Solutions**.

It demonstrates how an organisation can manage employee identities, organise users by department, assign access through security groups, and enforce the principle of least privilege.

The environment is deployed locally using Oracle VirtualBox.

## Architecture

| Component | Configuration |
|---|---|
| Domain Controller | IAM-DC01 |
| Server OS | Windows Server 2025 Evaluation |
| Active Directory Domain | ad.cybertech.test |
| DNS Server | Active Directory-integrated DNS |
| Network | VirtualBox Internal Network |
| Domain Controller IP | 192.168.50.10 |
| Virtualisation | Oracle VirtualBox 7.2.22 |

## Organisational Structure

The simulated organisation contains four departments:

- Information Technology (IT)
- Human Resources (HR)
- Finance
- Information Security

Departmental organisational units and security groups are configured in Active Directory.

## Implemented Features

- Windows Server 2025 domain controller deployment
- Active Directory Domain Services installation and configuration
- DNS Server deployment
- Creation of the `ad.cybertech.test` domain
- Departmental Organisational Units
- Fictional employee account provisioning
- Departmental Global Security Groups
- Employee-to-group membership assignment

## Technology Stack

- Windows Server 2025
- Active Directory Domain Services
- DNS Server
- PowerShell
- Python
- Oracle VirtualBox
- Git and GitHub

## Repository Structure

```text
Enterprise-IAM-Lab/
│
├── Documentation/
│   ├── Architecture.md
│   ├── Findings.md
│   └── Implementation-Log.md
│
├── Evidence/
│   ├── Screenshots/
│   │   ├── 01-Infrastructure-Setup/
│   │   ├── 02-Active-Directory-Deployment/
│   │   ├── 03-Organizational-Structure/
│   │   ├── 04-Identity-Provisioning/
│   │   └── 05-Group-Based-Access-Management/
│   │
│   └── Test-Results/
│
├── PowerShell/
├── Python/
├── Reports/
└── README.md
```

## Planned Implementation

The following components are yet to be implemented and validated:

- Department-specific shared folders
- NTFS and network share permissions
- Role-Based Access Control (RBAC) validation
- Least-privilege access testing
- Domain client authentication
- Group Policy security configuration
- Employee onboarding, transfer, and offboarding
- Account auditing and access reviews
- PowerShell automation
- Final security assessment and reporting

## Documentation

- [Architecture](Documentation/Architecture.md)
- [Implementation Log](Documentation/Implementation-Log.md)
- [Security Findings](Documentation/Findings.md)

## Security Scope

This project is conducted entirely within an authorised, isolated local virtual environment using fictional employee identities and test resources.

No production systems or real employee accounts are accessed.

---

**Project Status:** Active Development