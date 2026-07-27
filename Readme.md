For the **root** of your **Azure-Hybrid-Infrastructure-Lab** repository, don't make it like an individual lab. Instead, make it a **portfolio landing page** that showcases all labs. Recruiters will land here first.

Use this as your root `README.md`:

````markdown
<div align="center">

# ☁️ Azure Hybrid Infrastructure Lab

Building a real-world Microsoft Azure Hybrid Infrastructure from scratch using Azure Virtual Machines, Windows Server, Active Directory Domain Services, Azure Networking, DNS, Group Policy, Azure Bastion, and Hybrid Identity.

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-2022-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active%20Directory-AD%20DS-success?style=for-the-badge)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Status](https://img.shields.io/badge/Project-In%20Progress-brightgreen?style=for-the-badge)

</div>

---

# 📖 Project Overview

This repository contains a collection of hands-on Microsoft Azure Hybrid Infrastructure labs designed to simulate enterprise IT environments.

The labs cover the deployment and administration of Azure Virtual Machines, Active Directory Domain Services (AD DS), Azure Virtual Networking, Azure Bastion, DNS, Windows Server administration, Group Policy, and hybrid infrastructure concepts commonly used by System Administrators and Cloud Engineers.

Each lab includes detailed documentation, screenshots, implementation steps, verification procedures, and key learning outcomes.

---

# 🎯 Project Goals

- Deploy Azure Infrastructure
- Configure Virtual Networking
- Deploy Windows Server
- Install Active Directory Domain Services
- Configure DNS
- Join Windows Client Computers to Active Directory
- Implement Azure Bastion
- Configure Group Policy
- Manage Users and Organizational Units
- Build Enterprise Hybrid Infrastructure

---

# 🛠 Technologies Used

- Microsoft Azure
- Azure Virtual Machines
- Azure Virtual Network (VNet)
- Azure Bastion
- Windows Server 2022
- Active Directory Domain Services
- DNS
- PowerShell
- Windows Administration
- Networking
- Microsoft Entra ID (Future Labs)

---

# 🏗 Lab Architecture

```text
                     Microsoft Azure

                    Azure Resource Group
                           │
        ┌──────────────────┴──────────────────┐
        │                                     │
        │                                     │
 Azure Virtual Network                 Azure Bastion
      192.168.10.0/24                       │
        │                                   │
        │                                   │
┌──────────────┐                   Secure Browser RDP
│   SERVER01   │                          │
│Domain Control│                          │
│ Active Dir   │                          │
│ DNS Server   │                          │
└──────┬───────┘                          │
       │                                  │
       │                                  │
┌──────▼───────┐                          │
│   CLIENT01   │──────────────────────────┘
│ Domain Joined│
│ Windows VM   │
└──────────────┘
```

---

# 📚 Labs Completed

| Lab | Description | Status |
|------|-------------|--------|
| ✅ Lab 01 | Azure Resource Group | Completed |
| ✅ Lab 02 | Azure Virtual Network (VNet) | Completed |
| ✅ Lab 03 | Azure Virtual Machine Deployment | Completed |
| ✅ Lab 04 | Install Active Directory Domain Services | Completed |
| ✅ Lab 05 | Configure Azure Bastion | Completed |
| ✅ Lab 06 | Promote Windows Server to Domain Controller | Completed |
| ✅ Lab 07 | Configure DNS | Completed |
| ✅ Lab 08 | Join Windows Client to Active Directory Domain | Completed |

---

# 📂 Repository Structure

```text
Azure-Hybrid-Infrastructure-Lab
│
├── Lab 01 – Azure Resource Group
├── Lab 02 – Azure Virtual Network and Subnets
├── Lab 03 – Azure Virtual Machine Deployment
├── Lab 04 – Install Active Directory Domain Services
├── Lab 05 – Azure Bastion
├── Lab 06 – Promote Server to Domain Controller
├── Lab 07 – Configure DNS
├── Lab 08 – Join Windows Client to Active Directory Domain
└── README.md
```

---

# 💼 Skills Demonstrated

- Azure Infrastructure Deployment
- Windows Server Administration
- Active Directory Domain Services
- Azure Networking
- DNS Configuration
- Azure Bastion
- Windows Client Administration
- Active Directory Domain Join
- PowerShell
- Enterprise Troubleshooting
- Hybrid Infrastructure Administration

---

# 🚀 Upcoming Labs

- Active Directory Users and Computers (ADUC)
- Organizational Units (OU)
- User and Group Management
- Group Policy Objects (GPO)
- File Server
- Shared Folder Permissions
- NTFS Permissions
- DHCP Server
- Windows Server Backup
- Azure VPN Gateway
- Hybrid Identity with Microsoft Entra ID
- Azure File Sync
- Windows Admin Center

---

# 📜 Certifications Supported by These Labs

- Microsoft Certified: Azure Administrator Associate (AZ-104)
- Microsoft Certified: Azure Fundamentals (AZ-900)
- Windows Server Administration
- Active Directory Administration
- Microsoft Identity and Access Administrator (SC-300)

---

# 👨‍💻 Author

**Pavan Baburao Somwanshi**

**System Administrator | Azure | Windows Server | Active Directory | Microsoft 365 | Networking | Cloud Infrastructure**

📍 Pune, Maharashtra, India

GitHub: https://github.com/jaysomwanshi

---

<div align="center">

⭐ If you found this repository useful, consider giving it a **Star**.

</div>
````

This style is much more appropriate for the repository root because it acts as a portfolio homepage, while each lab has its own detailed `README.md`. It gives recruiters a clear overview of your Azure learning path and makes the repository easy to navigate.
