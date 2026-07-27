For your **root repository** `Azure-Hybrid-Infrastructure-Lab`, the main `README.md` should act as a portfolio landing page that explains the complete Azure hybrid infrastructure journey and links to individual labs.

Use this:

````markdown
# 🚀 Azure Hybrid Infrastructure Lab

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Cloud](https://img.shields.io/badge/Cloud-Infrastructure-blue?style=for-the-badge)
![Networking](https://img.shields.io/badge/Networking-VNet%20%7C%20VPN%20%7C%20Routing-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Progress-orange?style=for-the-badge)

A hands-on **Azure Hybrid Infrastructure implementation project** designed to simulate a real-world enterprise IT environment.

This repository documents my practical learning journey building Azure infrastructure components including networking, identity, security, hybrid connectivity, and cloud administration using Microsoft Azure.

---

# 📌 Project Overview

The goal of this project is to design and deploy a production-style Azure hybrid environment similar to what is used in enterprise organizations.

The lab focuses on:

- Azure Networking
- Virtual Networks (VNets)
- Subnet Design
- Network Security
- Hybrid Connectivity
- Identity Management
- Windows Server Infrastructure
- Cloud Administration
- Monitoring and Troubleshooting

---

# 🏗️ Target Architecture

```
                 Internet
                    |
                    |
             Azure Cloud Platform
                    |
              Azure Virtual Network
                    |
    -----------------------------------
    |                                 |
 Servers Subnet                 Client Subnet
    |                                 |
 Windows Servers              Client Machines
 Domain Services               Applications
 DNS / DHCP                    Testing
```

Future expansion:

```
On-Premises Data Center
          |
          |
     VPN Gateway
          |
          |
    Azure Virtual Network
```

---

# 🧪 Labs Included

## ✅ Lab 01 - Azure Resource Group & Environment Setup

**Objective:**

Create the foundation for Azure infrastructure deployment.

Topics covered:

- Azure Subscription management
- Resource Groups
- Azure Portal navigation
- Resource organization
- Deployment validation

Repository:

🔗 Coming Soon

---

# ✅ Lab 02 - Azure Virtual Network & Subnets

**Objective:**

Design Azure network architecture with proper IP addressing and subnet segmentation.

Topics covered:

- Azure Virtual Network creation
- CIDR planning
- Subnet design
- Private IP addressing
- Network segmentation
- Azure Layer 3 routing concepts


Repository:

🔗 [Azure VNet Subnets Lab](https://github.com/jaysomwanshi/azure-vnet-subnets-lab)


Network Design:

| Component | Address Range |
|---|---|
| Virtual Network | 192.168.10.0/24 |
| Servers Subnet | 192.168.10.0/26 |
| Clients Subnet | 192.168.10.64/26 |


---

# 🔜 Upcoming Labs

## Lab 03 - Azure Network Security Group (NSG)

Planned topics:

- Traffic filtering
- Security rules
- Inbound/outbound control
- Secure subnet access


---

## Lab 04 - Azure Virtual Machines

Topics:

- Windows Server deployment
- Linux VM deployment
- VM networking
- Disk management
- Remote administration


---

## Lab 05 - Azure Bastion Host

Topics:

- Secure RDP/SSH access
- Eliminating public IP exposure
- Cloud administration best practices


---

## Lab 06 - Azure VPN Gateway Hybrid Connectivity

Topics:

- Site-to-site VPN
- Hybrid networking
- On-premises simulation
- Secure connectivity


---

## Lab 07 - Active Directory Hybrid Identity

Topics:

- Windows Server Domain Controller
- Active Directory Domain Services
- DNS integration
- Azure Entra ID synchronization


---

## Lab 08 - Azure Monitoring & Security

Topics:

- Azure Monitor
- Log Analytics
- Security recommendations
- Resource health monitoring


---

# 🛠️ Technologies Used

## Microsoft Azure

- Azure Virtual Network
- Azure Virtual Machines
- Azure Resource Groups
- Azure Bastion
- Azure VPN Gateway
- Azure Monitor
- Microsoft Entra ID


## Networking

- IPv4 Addressing
- CIDR Subnetting
- Routing Concepts
- VLAN Concepts
- NAT
- DNS
- DHCP


## Operating Systems

- Windows Server
- Windows Client
- Linux


## Administration Tools

- Azure Portal
- PowerShell
- Azure CLI
- Remote Desktop
- SSH


---

# 🎯 Skills Demonstrated

This project demonstrates practical knowledge in:

✅ Cloud Infrastructure Deployment  
✅ Azure Networking  
✅ IP Address Planning  
✅ Enterprise Network Design  
✅ Windows Server Administration  
✅ Hybrid Cloud Concepts  
✅ Security Fundamentals  
✅ Troubleshooting Methodology  
✅ Documentation Skills  


---

# 📸 Screenshots

Screenshots for each lab are stored inside individual repositories.

Example:

```
azure-vnet-subnets-lab
│
├── screenshots
│   ├── 01-azure-dashboard.png
│   ├── 02-vnet-created.png
│   ├── 03-subnet-config.png
│
└── README.md
```

---

# 📚 Learning Objectives

By completing this project, I aim to build practical expertise in:

- Designing Azure enterprise networks
- Deploying secure cloud infrastructure
- Understanding hybrid environments
- Managing Windows and Linux workloads
- Preparing for real-world Cloud/System Administrator roles


---

# 👨‍💻 Author

**Jay Somwanshi**

System Administrator | Cloud Infrastructure Learner

Skills:

- Microsoft Azure
- Windows Server
- Active Directory
- Networking
- Linux
- AWS
- Cloud Automation


---

# ⭐ Project Status

🚧 **Active Development**

New Azure infrastructure labs will be added regularly as the environment expands.

---

# 📖 References

Microsoft Azure Documentation:

https://learn.microsoft.com/azure/

Azure Architecture Center:

https://learn.microsoft.com/azure/architecture/
````

This root README will look like a **cloud engineer portfolio repository**, not just a lab dump. It will also connect all future labs cleanly as you add them.
