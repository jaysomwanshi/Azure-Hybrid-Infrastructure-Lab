````markdown
# Lab 08 – Join Windows Client Virtual Machine to Active Directory Domain

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server-2022-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active%20Directory-Domain%20Services-003366?style=for-the-badge)
![DNS](https://img.shields.io/badge/DNS-Configured-success?style=for-the-badge)
![PowerShell](https://img.shields.io/badge/PowerShell-5.1-5391FE?style=for-the-badge&logo=powershell)

---

# Overview

This lab demonstrates how to deploy a Windows client virtual machine in Microsoft Azure and join it to an existing Active Directory Domain Services (AD DS) environment hosted on **SERVER01**.

The client machine was connected securely using **Azure Bastion**, configured to use the Domain Controller's DNS server, and successfully joined to the **corp.local** Active Directory domain.

This lab represents a common enterprise task performed by System Administrators when provisioning new computers into an organization's domain environment.

---

# Objectives

- Deploy a Windows client virtual machine in Azure
- Connect securely using Azure Bastion
- Configure the computer name
- Join the client to the Active Directory domain
- Authenticate using Domain Administrator credentials
- Verify successful domain membership

---

# Lab Environment

| Component | Details |
|-----------|---------|
| Cloud Platform | Microsoft Azure |
| Domain Controller | SERVER01 |
| Domain | corp.local |
| Client Computer | CLIENT01 |
| Authentication | Domain Administrator |
| Remote Access | Azure Bastion |
| Directory Service | Active Directory Domain Services |
| DNS | Hosted on SERVER01 |

---

# Architecture

```
                    Microsoft Azure

             +-------------------------+
             |      Azure VNet         |
             |   192.168.10.0/24       |
             +-----------+-------------+
                         |
        -----------------------------------------
        |                                       |
+---------------------+               +---------------------+
|      SERVER01       |               |      CLIENT01       |
| Domain Controller   |<------------->| Windows Client VM   |
| Active Directory    |               | Domain Joined       |
| DNS Server          |               | Azure Bastion       |
+---------------------+               +---------------------+

                 Domain: corp.local
```

---

# Prerequisites

- Existing Azure Subscription
- Active Directory Domain Services installed
- SERVER01 promoted as Domain Controller
- DNS configured correctly
- Azure Bastion deployed
- Windows Client virtual machine created

---

# Implementation Steps

## Step 1 — Deploy Windows Client VM

- Created a new Windows client virtual machine
- Selected the existing Resource Group
- Configured networking
- Validated deployment

---

## Step 2 — Connect via Azure Bastion

- Connected securely without exposing RDP publicly
- Verified successful login

---

## Step 3 — Configure Computer Name

Opened:

```
sysdm.cpl
```

Navigated to:

```
Computer Name
```

Changed the computer configuration before joining the domain.

---

## Step 4 — Join Active Directory Domain

Selected:

```
Domain
```

Entered:

```
corp.local
```

Authenticated using Domain Administrator credentials.

---

## Step 5 — Verify Domain Join

Successful confirmation message displayed:

```
Welcome to the corp.local domain.
```

Restarted the virtual machine to complete the domain join process.

---

# Verification

After restart verify:

```powershell
whoami
```

Check domain membership:

```cmd
systeminfo | findstr /B /C:"Domain"
```

Verify computer information:

```cmd
hostname
```

Verify secure channel:

```cmd
nltest /sc_verify:corp.local
```

---

# Skills Demonstrated

- Microsoft Azure
- Azure Virtual Machines
- Azure Bastion
- Windows Administration
- Active Directory Domain Services
- Domain Join
- DNS Configuration
- Windows Networking
- Enterprise Authentication
- Identity Management

---

# Screenshots

| Step | Screenshot |
|------|------------|
| Azure Portal Dashboard | ![](screenshots/01-azure-portal-dashboard.png) |
| SERVER01 Overview | ![](screenshots/02-server01-overview.png) |
| Create Client VM | ![](screenshots/03-create-client01-vm.png) |
| VM Configuration | ![](screenshots/04-client01-vm-configuration.png) |
| Validation Passed | ![](screenshots/05-validation-passed.png) |
| Deployment Progress | ![](screenshots/06-deployment-progress.png) |
| CLIENT01 Overview | ![](screenshots/07-client01-overview.png) |
| Azure Bastion Connection | ![](screenshots/08-client01-bastion-connection.png) |
| Domain Join Settings | ![](screenshots/09-domain-join-settings.png) |
| Computer Name Configuration | ![](screenshots/10-computer-name-change.png) |
| Domain Credentials | ![](screenshots/11-domain-credentials.png) |
| Domain Join Successful | ![](screenshots/12-domain-join-success.png) |
| Restart Required | ![](screenshots/13-restart-required.png) |

---

# Troubleshooting

### Unable to locate the domain

- Verify DNS points to the Domain Controller.
- Confirm network connectivity to SERVER01.
- Ensure required firewall ports are open.

### Authentication Failed

- Verify Domain Administrator credentials.
- Ensure the client can resolve the domain using DNS.

### Domain Join Failed

- Confirm Active Directory Domain Services is healthy.
- Verify the computer name is unique.
- Restart the client after joining.

---

# Learning Outcomes

After completing this lab, you can:

- Deploy Azure virtual machines
- Connect securely using Azure Bastion
- Join Windows systems to Active Directory
- Authenticate with Domain Administrator credentials
- Verify successful domain membership
- Troubleshoot common domain join issues

---

# Repository Structure

```
Lab 08 – Join Windows Client Virtual Machine to Active Directory Domain
│
├── README.md
└── screenshots
    ├── 01-azure-portal-dashboard.png
    ├── 02-server01-overview.png
    ├── 03-create-client01-vm.png
    ├── 04-client01-vm-configuration.png
    ├── 05-validation-passed.png
    ├── 06-deployment-progress.png
    ├── 07-client01-overview.png
    ├── 08-client01-bastion-connection.png
    ├── 09-domain-join-settings.png
    ├── 10-computer-name-change.png
    ├── 11-domain-credentials.png
    ├── 12-domain-join-success.png
    └── 13-restart-required.png
```

---

# Conclusion

This lab demonstrated the end-to-end process of deploying a Windows client virtual machine in Microsoft Azure and successfully joining it to an existing Active Directory domain. It covered secure remote administration with Azure Bastion, domain authentication, DNS dependency, and post-join verification, reflecting a common enterprise System Administrator workflow.

---

## Author

**Jay Somwanshi**

**Role:** System Administrator | Azure | Windows Server | Active Directory | Microsoft 365 | Networking | Cloud Infrastructure

---
````
