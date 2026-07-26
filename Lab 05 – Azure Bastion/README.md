# Lab 05 – Azure Bastion

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Azure Bastion](https://img.shields.io/badge/Azure-Bastion-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📖 Overview

This lab demonstrates how to deploy **Azure Bastion**, a fully managed Platform-as-a-Service (PaaS) solution that provides secure browser-based Remote Desktop (RDP) and SSH connectivity to Azure Virtual Machines without exposing port **3389** or **22** to the public Internet.

Instead of connecting directly through a Public IP, Azure Bastion establishes secure connectivity over **HTTPS (TCP 443)** through the Azure Portal.

---

# 🎯 Objectives

- Deploy Azure Bastion
- Configure AzureBastionSubnet
- Create Bastion Public IP
- Secure Remote Desktop Access
- Connect to Azure VM through Browser
- Eliminate Direct Public RDP Access
- Improve Azure Network Security

---

# 🛠 Azure Services Used

- Azure Bastion
- Azure Virtual Machine
- Azure Virtual Network
- AzureBastionSubnet
- Public IP Address
- Network Security Group (NSG)

---

# 🌐 Lab Configuration

| Resource | Value |
|-----------|-------|
| Resource Group | RG-HybridLab |
| Bastion Name | bastion-hq |
| Region | Central India |
| Tier | Standard |
| Instance Count | 2 |
| Virtual Network | vnet-hq-001 |
| Bastion Subnet | AzureBastionSubnet (/26) |
| Virtual Machine | Server01 |
| Connection Type | Browser-based RDP |

---

# 🏗 Architecture

```text
                 Internet
                     │
              HTTPS (TCP 443)
                     │
              Azure Portal
                     │
             Azure Bastion
                     │
        AzureBastionSubnet (/26)
                     │
              vnet-hq-001
                     │
                Server01 VM
```

---

# 📸 Step 1 – Azure Portal Dashboard

![Dashboard](screenshots/01-dashboard.png)

---

# 📸 Step 2 – Search Azure Bastion

![Search Bastion](screenshots/02-search-bastion.png)

---

# 📸 Step 3 – Open Azure Bastion Service

![Open Bastion](screenshots/03-open-bastion.png)

---

# 📸 Step 4 – Create Azure Bastion

![Create Bastion](screenshots/04-create-bastion.png)

---

# 📸 Step 5 – Configure Basic Settings

- Resource Group
- Bastion Name
- Region
- Tier

![Basic Settings](screenshots/05-basic-settings.png)

---

# 📸 Step 6 – Configure Networking

- Virtual Network
- AzureBastionSubnet
- Public IP Address

![Network Settings](screenshots/06-network-settings.png)

---

# 📸 Step 7 – Validation Passed

![Validation Passed](screenshots/07-validation-passed.png)

---

# 📸 Step 8 – Deployment in Progress

![Deployment Progress](screenshots/08-deployment-progress.png)

---

# 📸 Step 9 – Deployment Completed Successfully

![Deployment Complete](screenshots/09-deployment-complete.png)

---

# 📸 Step 10 – AzureBastionSubnet Created

![AzureBastionSubnet](screenshots/10-azurebastionsubnet.png)

---

# 📸 Step 11 – Connect to Server01

The Azure Bastion connection page is used to enter the VM credentials and establish a secure browser-based Remote Desktop session.

![Connect Server01](screenshots/11-connect-server01.png)

---

# 📸 Step 12 – Browser-based Remote Desktop

Azure Bastion successfully connects to the Windows Server virtual machine directly within the Azure Portal without exposing RDP over the Internet.

![Browser RDP](screenshots/12-browser-rdp.png)

---

# 📸 Step 13 – Successful Azure Bastion Session

A successful browser-based RDP session to **Server01** through Azure Bastion confirms secure remote administration without requiring a Public RDP endpoint.

![Final Bastion Session](screenshots/13-bastion-final-lab.PNG)

---

# 🔒 Security Benefits

- Browser-based Remote Desktop
- No Public RDP Port (3389)
- Secure HTTPS (443) Connectivity
- Managed Microsoft PaaS Service
- Reduces Attack Surface
- Protects Azure Virtual Machines
- Simplifies Secure Remote Administration

---

# 📚 Skills Demonstrated

- Azure Bastion Deployment
- Azure Virtual Networking
- AzureBastionSubnet Configuration
- Secure Remote Administration
- Windows Server Remote Management
- Azure Infrastructure Security
- Network Security Best Practices

---

# ✅ Lab Outcome

Successfully deployed Azure Bastion and securely connected to the **Server01** Azure Virtual Machine using browser-based Remote Desktop without exposing RDP directly to the Internet.

---

# 🚀 Next Lab

**Lab 06 – Active Directory Domain Services (AD DS)**

Topics include:

- Active Directory Domain Services
- DNS Configuration
- Domain Controller
- Organizational Units (OU)
- Users & Groups
- Group Policy Objects (GPO)

---

# 👨‍💻 Author

**Pavan Baburao Somwanshi**

**System Administrator | Azure | Windows Server | Microsoft 365 | Networking | Cloud Computing**

GitHub: https://github.com/jaysomwanshi

---

⭐ If you found this project helpful, consider giving the repository a **Star**.
