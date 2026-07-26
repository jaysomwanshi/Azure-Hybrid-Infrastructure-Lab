# Azure Network Security Groups (NSG) Lab

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Security](https://img.shields.io/badge/Azure-Network%20Security-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📖 Overview

This lab demonstrates how to create and configure Azure Network Security Groups (NSGs) to secure Azure Virtual Machines. The lab covers creating an NSG, configuring inbound security rules, associating the NSG with a subnet, and verifying connectivity using Remote Desktop Protocol (RDP).

---

# 🎯 Objectives

- Create an Azure Network Security Group
- Configure inbound security rules
- Allow Remote Desktop (RDP)
- Allow HTTP traffic
- Allow HTTPS traffic
- Associate NSG with a subnet
- Verify VM connectivity
- Understand NSG rule priority

---

# 🛠 Azure Services Used

- Azure Virtual Network
- Azure Subnet
- Azure Network Security Group (NSG)
- Azure Virtual Machine
- Azure Network Interface
- Public IP Address

---

# 🌐 Lab Environment

| Resource | Configuration |
|----------|---------------|
| Resource Group | RG-HybridLab |
| Virtual Network | vnet-hq-001 |
| Subnet | Servers (192.168.10.0/26) |
| Virtual Machine | Server01 |
| NSG | NSG-Servers |

---

# 🗺 Network Topology

```text
                    Internet
                        │
                 Public IP Address
                        │
                  Azure Virtual Machine
                     Server01
                        │
                Network Interface (NIC)
                        │
      ----------------------------------------
      |                                      |
      |        NSG-Servers (Subnet)          |
      |                                      |
      ----------------------------------------
                        │
                Servers Subnet
             192.168.10.0/26
                        │
              vnet-hq-001 (VNet)
```

---

# 🔒 Configured Security Rules

| Priority | Port | Protocol | Action | Purpose |
|----------:|-----:|---------|--------|---------|
| 100 | 3389 | TCP | Allow | Remote Desktop |
| 110 | 80 | TCP | Allow | HTTP |
| 120 | 443 | TCP | Allow | HTTPS |

---

# 📸 Step 1 – Azure Dashboard

![Step 1](screenshots/01-dashboard.png)

---

# 📸 Step 2 – Open Network Settings

![Step 2](screenshots/02-network-settings.png)

---

# 📸 Step 3 – Search Network Security Groups

![Step 3](screenshots/03-network-security-groups.png)

---

# 📸 Step 4 – Create NSG

![Step 4](screenshots/04-create-nsg.png)

---

# 📸 Step 5 – Validation Passed

![Step 5](screenshots/05-nsg-validation-passed.png)

---

# 📸 Step 6 – Deployment Complete

![Step 6](screenshots/06-deployment-complete.png)

---

# 📸 Step 7 – NSG Overview

![Step 7](screenshots/07-nsg-overview.png)

---

# 📸 Step 8 – Inbound Security Rules

![Step 8](screenshots/08-inbound-rules.png)

---

# 📸 Step 9 – Add RDP Rule

![Step 9](screenshots/09-add-rdp-rule.png)

---

# 📸 Step 10 – RDP Rule Created

![Step 10](screenshots/10-rdp-rule-created.png)

---

# 📸 Step 11 – Add HTTP Rule

![Step 11](screenshots/11-add-http-rule.png)

---

# 📸 Step 12 – HTTP Rule Created

![Step 12](screenshots/12-http-rule-created.png)

---

# 📸 Step 13 – Add HTTPS Rule

![Step 13](screenshots/13-add-https-rule.png)

---

# 📸 Step 14 – HTTPS Rule Created

![Step 14](screenshots/14-https-rule-created.png)

---

# 📸 Step 15 – Verify Inbound Rules

![Step 15](screenshots/15-inbound-rules-overview.png)

---

# 📸 Step 16 – Open Subnet Association

![Step 16](screenshots/16-subnet-association.png)

---

# 📸 Step 17 – Associate NSG with Servers Subnet

![Step 17](screenshots/17-associate-subnet.png)

---

# 📸 Step 18 – Association Complete

![Step 18](screenshots/18-subnet-associated.png)

---

# 📸 Step 19 – Verify Server01 Network Interface

![Step 19](screenshots/19-server01-nic.png)

---

# 📸 Step 20 – Verify Effective Security Rules

![Step 20](screenshots/20-effective-security-rules.png)

---

# 📸 Step 21 – Remote Desktop Connection

![Step 21](screenshots/21-rdp-connected.png)

---

# 💡 What I Learned

✅ Azure Network Security Groups (NSGs)

✅ Inbound Security Rules

✅ Security Rule Priorities

✅ RDP Access Configuration

✅ HTTP & HTTPS Access

✅ Subnet-Level Security

✅ Network Interface Verification

✅ Effective Security Rules

✅ Secure Azure Networking

---

# 📚 Key Concepts

### What is an NSG?

An Azure Network Security Group (NSG) is a virtual firewall that filters inbound and outbound network traffic for Azure resources.

### Rule Processing

Azure processes NSG rules based on **Priority**. Lower numbers are evaluated before higher numbers.

Example:

- Priority **100** → RDP
- Priority **110** → HTTP
- Priority **120** → HTTPS

If no rule matches, Azure applies the default **DenyAllInbound** rule.

---

# 🚀 Next Lab

- Azure Bastion
- Secure RDP without Public Ports
- Azure Storage Accounts
- Azure Files
- Azure Load Balancer

---

# 👨‍💻 Author

**Pavan Baburao Somwanshi**

System Administrator | Azure | Windows Server | Networking | Cloud

GitHub: https://github.com/jaysomwanshi

---

⭐ If you found this project useful, consider giving it a Star!

