# Azure Virtual Machines (VM) Deployment Lab

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Compute](https://img.shields.io/badge/Azure-Virtual%20Machines-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📖 Overview

This lab demonstrates how to deploy a Windows Server virtual machine in Microsoft Azure using an existing Resource Group and Virtual Network. The lab covers VM sizing, networking, remote connectivity, and deployment validation.

---

# 🎯 Objectives

- Deploy an Azure Virtual Machine
- Select VM size and image
- Configure administrator credentials
- Connect VM to an existing Virtual Network
- Enable Remote Desktop (RDP)
- Verify Public and Private IP configuration
- Connect successfully using RDP

---

# 🛠 Azure Services Used

- Azure Resource Groups
- Azure Virtual Machines
- Azure Virtual Network (VNet)
- Azure Network Interface (NIC)
- Azure Public IP Address
- Network Security Group (NSG)
- Managed Disks

---

# 🌐 Lab Architecture

```text
Internet
    │
Public IP
    │
┌──────────────────────┐
│      Server01        │
│ Windows Server 2025  │
└──────────┬───────────┘
           │
      Network Interface
           │
Azure Virtual Network
192.168.10.0/24
           │
Servers Subnet
192.168.10.0/26
```

---

# ⚙ VM Configuration

| Setting | Value |
|---------|-------|
| Virtual Machine | Server01 |
| Operating System | Windows Server 2025 Datacenter Azure Edition |
| Region | Central India |
| Virtual Network | Existing VNet |
| Subnet | Servers |
| Authentication | Username & Password |
| Remote Access | RDP (3389) |

---

# 📸 Step 1 - Azure Dashboard

![Dashboard](screenshots/01-dashboard.png)

---

# 📸 Step 2 - Search Virtual Machines

![Search](screenshots/02-search-virtual-machines.png)

---

# 📸 Step 3 - Open Compute Services

![Compute](screenshots/03-compute-services.png)

---

# 📸 Step 4 - Select Virtual Machine

![Virtual Machine](screenshots/04-select-virtual-machine.png)

---

# 📸 Step 5 - Create Virtual Machine

![Create VM](screenshots/05-create-vm.png)

---

# 📸 Step 6 - Select Resource Group

![Resource Group](screenshots/06-resource-group.png)

---

# 📸 Step 7 - Configure VM Basics

![Basics](screenshots/07-basics.png)

---

# 📸 Step 8 - Select Operating System Image

![Image](screenshots/08-image-selection.png)

---

# 📸 Step 9 - Configure VM Size & Administrator

![VM Size](screenshots/09-vm-size-admin-account.png)

---

# 📸 Step 10 - Configure RDP & Review

![Review](screenshots/10-rdp-review-create.png)

---

# 📸 Step 11 - Validation Passed

![Validation](screenshots/11-validation-passed.png)

---

# 📸 Step 12 - Deployment Complete

![Deployment](screenshots/12-deployment-complete.png)

---

# 📸 Step 13 - Server01 Overview

![Overview](screenshots/13-server01-overview.png)

---

# 📸 Step 14 - Network Interface

![Network Interface](screenshots/14-network-interface.png)

---

# 📸 Step 15 - Network Security Group

![NSG](screenshots/15-network-security-group.png)

---

# 📸 Step 16 - Download RDP File

![RDP](screenshots/16-download-rdp.png)

---

# 📸 Step 17 - Remote Desktop Connected

![Connected](screenshots/17-rdp-connected.png)

---

# 💡 What I Learned

✅ Azure Virtual Machine deployment

✅ VM sizing and image selection

✅ Administrator account configuration

✅ Virtual Network integration

✅ Public and Private IP addressing

✅ Network Security Groups (NSG)

✅ Remote Desktop Protocol (RDP)

✅ Azure compute resource management

---

# 🚀 Next Lab

- Azure Network Security Groups (NSG)
- NSG Rules (Inbound & Outbound)
- Secure RDP Access
- Application Security Groups (ASG)

---

# 👨‍💻 Author

**Pavan Baburao Somwanshi**

System Administrator | Azure | Windows Server | Networking | Cloud

GitHub: https://github.com/jaysomwanshi

---

⭐ If you found this project useful, consider giving it a Star!
