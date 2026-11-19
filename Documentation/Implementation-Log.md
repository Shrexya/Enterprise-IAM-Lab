# Implementation Log

## Project: Enterprise Identity & Access Management Lab

### 14 November 2026 — Initial Preparation

#### Environment Assessment
- Verified Windows host and 64-bit architecture.
- Verified approximately 15.38 GB RAM.
- Verified 16 logical processors.
- Verified 318.73 GB free storage.
- Verified VirtualBox 7.2.22.
- Identified the existing SOC-Ubuntu-SIEM virtual machine.

#### Repository Setup
- Cloned the GitHub repository.
- Created the project directory structure.
- Created the initial documentation files.
- Prepared the IAM architecture.

### 18–19 November 2026 — Infrastructure and Active Directory Deployment

#### Virtual Machine Configuration
- Created the `IAM-DC01` virtual machine.
- Installed Windows Server 2025 Standard Evaluation (Desktop Experience).
- Configured 6 GB RAM, 2 virtual CPUs and an 80 GB virtual disk.
- Renamed the server to `IAM-DC01`.
- Configured an isolated VirtualBox Internal Network named `IAM-Internal`.
- Assigned static IPv4 address `192.168.50.10/24`.

#### Active Directory and DNS Deployment
- Installed Active Directory Domain Services (AD DS).
- Installed the DNS Server role.
- Promoted `IAM-DC01` to a domain controller.
- Created a new Active Directory forest with the domain `ad.cybertech.test`.
- Verified the domain configuration.
- Verified that the DNS and NTDS services were running.

#### Organisational Structure
- Created the parent organisational unit `CyberTech Solutions`.
- Created department OUs:
  - IT
  - HR
  - Finance
  - Information Security

#### Identity Provisioning
Created the following employee accounts:

| Employee | Department | Username |
|---|---|---|
| Rahul Sharma | IT | rahul.sharma |
| Priya Das | HR | priya.das |
| Arjun Roy | Finance | arjun.roy |
| Neha Sen | Information Security | neha.sen |

#### Group-Based Access Management
Created the following Global Security Groups:
- `GG_IT`
- `GG_HR`
- `GG_Finance`
- `GG_InfoSec`

Assigned employees to their corresponding departmental security groups.

#### Evidence Collection
- Captured screenshots of server and domain configuration.
- Captured the Active Directory organisational structure.
- Captured employee account details.
- Captured group membership evidence.
- Organised screenshots in the repository's Evidence directory.

### Current Implementation Status

**Completed**
- Virtual infrastructure setup.
- Active Directory and DNS deployment.
- Domain controller configuration.
- Organisational unit creation.
- Employee identity provisioning.
- Departmental security group creation and membership assignment.

**Pending**
- Shared folder and NTFS permission configuration.
- Authentication and access-control testing.
- Group Policy configuration.
- Identity lifecycle management.
- Security auditing and monitoring.
- PowerShell automation and final reporting.

### Next Implementation Objective

Configure department-specific shared resources and enforce access through security groups, following the principle of least privilege.

*Note: Authentication, authorisation and security-control testing have not yet been completed.*