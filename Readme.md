# ☁️ Azure Hybrid Infrastructure Labs

![Azure](https://img.shields.io/badge/Microsoft%20Azure-Cloud-blue)
![Status](https://img.shields.io/badge/Labs-In%20Progress-orange)

## 📌 Project Overview

This project contains my hands-on **Azure Hybrid Infrastructure Labs** where I built and configured a basic enterprise cloud environment.

The purpose of this project is to understand the fundamentals of Azure infrastructure, networking, security, and secure remote administration.

The labs cover:

- Azure Resource Management
- Virtual Networks
- Subnet Design
- Network Security Groups
- Azure Bastion
- Secure VM Access

---

# 🏗️ Azure Infrastructure Flow

```

Azure Subscription

```
    |
    |
```

Resource Group

```
    |
    |
```

Virtual Network (VNet)

```
    |
    |
```

Subnets

```
    |
    |
```

Network Security Groups

```
    |
    |
```

Azure Resources
(Virtual Machines / Bastion)

```

---

# 📚 Lab Progress

| Lab | Topic | Status |
|-----|-------|--------|
| Lab 01 | Azure Subscription & Resource Group | ✅ Completed |
| Lab 02 | Azure Virtual Network (VNet) | ✅ Completed |
| Lab 03 | Subnet Creation & IP Planning | ✅ Completed |
| Lab 04 | Network Security Group (NSG) | ✅ Completed |
| Lab 05 | Azure Bastion Secure Access | ✅ Completed |
| Lab 06 | Azure Virtual Machine Deployment | ⏳ Pending |
| Lab 07 | Active Directory Domain Controller | ⏳ Pending |
| Lab 08 | Azure VPN Gateway Hybrid Connection | ⏳ Pending |
| Lab 09 | Azure Monitoring & Backup | ⏳ Pending |

---

# ✅ Completed Labs

## Lab 01 - Resource Group Creation

### Objective

Create a logical container to organize Azure resources.

### Implementation

Created Resource Group:

```

RG-HybridLab

```

Resource Groups help manage related Azure services together.

Example:

```

RG-HybridLab

|
|-- Virtual Network
|-- Network Security Group
|-- Virtual Machines
|-- Bastion

```

### Screenshot

![Resource Group](screenshots/resource-group.png)

---

# Lab 02 - Virtual Network Creation

### Objective

Create a private network environment inside Azure.

### Implementation

Created:

```

VNet Name:

Hybrid-VNet

Address Space:

192.168.10.0/24

```

The Virtual Network provides the private IP address range for Azure resources.

### Screenshot

![Virtual Network](screenshots/vnet.png)

---

# Lab 03 - Subnet Design

### Objective

Divide the Virtual Network into smaller network segments.

Created subnets:

## Servers Subnet

```

192.168.10.0/26

```

Purpose:

- Server workloads
- Infrastructure services


## Clients Subnet

```

192.168.10.64/26

```

Purpose:

- Client machines
- Testing systems


## Azure Bastion Subnet

```

AzureBastionSubnet

192.168.10.128/27

```

Purpose:

- Secure VM administration


### Screenshot

![Subnets](screenshots/subnets.png)

---

# Lab 04 - Network Security Group (NSG)

### Objective

Control inbound and outbound network traffic.

Configured security rules:

Example:

```

Inbound:

Allow RDP
TCP 3389

Allow HTTPS
TCP 443

```

NSG works as a cloud firewall by controlling:

- Source
- Destination
- Port
- Protocol
- Allow/Deny Rules


### Screenshot

![NSG](screenshots/nsg.png)

---

# Lab 05 - Azure Bastion

### Objective

Provide secure access to Azure Virtual Machines without exposing them directly to the internet.

### Connection Flow

```

Administrator Laptop

```
    |
    |
 HTTPS 443

    |
    |
```

Azure Bastion

```
    |
    |
```

Private VM

192.168.10.x

```

Benefits:

✅ No direct public RDP exposure  
✅ Secure browser-based access  
✅ Private VM connectivity  
✅ Reduced attack surface  


### Screenshot

![Azure Bastion](screenshots/bastion.png)

---

# 📂 Repository Structure

```

Azure-Hybrid-Infrastructure-Labs

│
├── Lab-01-Resource-Group
│
├── Lab-02-Virtual-Network
│
├── Lab-03-Subnet-Configuration
│
├── Lab-04-Network-Security-Group
│
├── Lab-05-Azure-Bastion
│
├── screenshots
│
└── README.md

```

---

# 🛠️ Skills Demonstrated

- Azure Subscription Management
- Resource Group Management
- Virtual Network Design
- IPv4 Address Planning
- Subnetting
- Network Security Groups
- Firewall Rules
- Azure Bastion Deployment
- Cloud Infrastructure Fundamentals

---

# 🚀 Upcoming Labs

Future implementation:

⏳ Azure Virtual Machine Deployment  
⏳ Windows Server Configuration  
⏳ Active Directory Domain Services  
⏳ Azure DNS  
⏳ VPN Gateway Hybrid Connectivity  
⏳ Azure Monitoring and Backup  

---

# 👨‍💻 Author

**Jay Somwanshi**

System Administrator | Azure Infrastructure Learner

GitHub:
https://github.com/jaysomwanshi
```

This version is cleaner for a recruiter:

* Easy first read
* Shows architecture
* Shows progress
* Shows screenshots
* Does not look like copied documentation
* Matches your actual labs completed so far.
