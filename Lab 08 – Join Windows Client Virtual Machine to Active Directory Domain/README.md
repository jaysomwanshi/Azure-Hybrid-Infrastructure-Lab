# Join Windows Client Virtual Machine to Active Directory Domain

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Windows](https://img.shields.io/badge/Windows-Client-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Active%20Directory](https://img.shields.io/badge/Active%20Directory-Domain%20Join-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

# 📖 Overview

This lab demonstrates how to deploy a Windows client virtual machine in Microsoft Azure and successfully join it to an existing **Active Directory Domain Services (AD DS)** environment.

The client virtual machine communicates with the Domain Controller using Azure Virtual Network and DNS, authenticates with domain credentials, and becomes a member of the **corp.local** Active Directory domain.

This is one of the most common tasks performed by Windows System Administrators in enterprise environments.

---

# 🎯 Objectives

- Deploy a Windows Client Virtual Machine
- Connect using Azure Bastion
- Configure Computer Name
- Join Active Directory Domain
- Authenticate using Domain Administrator Credentials
- Verify Successful Domain Membership

---

# 🛠 Azure Services Used

- Azure Resource Group
- Azure Virtual Machine
- Azure Virtual Network (VNet)
- Azure Bastion
- Active Directory Domain Services
- Azure DNS (Private)

---

# 🌐 Lab Environment

| Component | Configuration |
|-----------|---------------|
| Domain | corp.local |
| Domain Controller | SERVER01 |
| Client Computer | CLIENT01 |
| Operating System | Windows Client |
| Authentication | Domain Administrator |
| Remote Access | Azure Bastion |

---

# 🗺 Architecture

```text
                   Azure Virtual Network
                      192.168.10.0/24
                              │
          ┌───────────────────┴───────────────────┐
          │                                       │
          │                                       │
 ┌──────────────────────┐              ┌──────────────────────┐
 │      SERVER01        │              │      CLIENT01        │
 │ Domain Controller    │◄────────────►│ Windows Client VM    │
 │ Active Directory     │              │ Joined to Domain     │
 │ DNS Server           │              │ Azure Bastion Access │
 └──────────────────────┘              └──────────────────────┘

                    Domain: corp.local
```

---

# 📸 Step 1 - Azure Portal Dashboard

![Azure Dashboard](screenshots/01-azure-portal-dashboard.png)

---

# 📸 Step 2 - SERVER01 Overview

![SERVER01 Overview](screenshots/02-server01-overview.png)

---

# 📸 Step 3 - Create Client Virtual Machine

![Create VM](screenshots/03-create-client01-vm.png)

---

# 📸 Step 4 - Configure Virtual Machine

![VM Configuration](screenshots/04-client01-vm-configuration.png)

---

# 📸 Step 5 - Validation Passed

![Validation](screenshots/05-validation-passed.png)

---

# 📸 Step 6 - Deployment Progress

![Deployment Progress](screenshots/06-deployment-progress.png)

---

# 📸 Step 7 - CLIENT01 Virtual Machine Overview

![Client Overview](screenshots/07-client01-overview.png)

---

# 📸 Step 8 - Connect Using Azure Bastion

![Azure Bastion](screenshots/08-client01-bastion-connection.png)

---

# 📸 Step 9 - Open Domain Join Settings

![Domain Join Settings](screenshots/09-domain-join-settings.png)

---

# 📸 Step 10 - Configure Computer Name

![Computer Name](screenshots/10-computer-name-change.png)

---

# 📸 Step 11 - Enter Domain Administrator Credentials

![Credentials](screenshots/11-domain-credentials.png)

---

# 📸 Step 12 - Domain Join Successful

![Success](screenshots/12-domain-join-success.png)

---

# 📸 Step 13 - Restart Client

![Restart Required](screenshots/13-restart-required.png)

---

# ✅ Verification

After restarting the virtual machine, verify the domain join.

Open **Command Prompt** and run:

```cmd
hostname
```

```cmd
whoami
```

```cmd
systeminfo | findstr /B /C:"Domain"
```

```cmd
nltest /sc_verify:corp.local
```

Expected Result:

- Computer is joined to **corp.local**
- Secure channel verification succeeds
- Domain authentication is operational

---

# 💡 What I Learned

✅ Deploy Azure Virtual Machines

✅ Configure Azure Bastion

✅ Join Windows Client to Active Directory

✅ Configure Domain Authentication

✅ Windows Computer Name Configuration

✅ Active Directory Domain Membership

✅ Enterprise Identity Management

---

# 🚀 Next Lab

- Active Directory Users and Computers (ADUC)
- Organizational Units (OU)
- User & Group Management
- Group Policy Objects (GPO)
- DNS Management
- Shared Folder Permissions

---

# 👨‍💻 Author

**Pavan Baburao Somwanshi**

System Administrator | Azure | Windows Server | Active Directory | Microsoft 365 | Networking | Cloud Infrastructure

GitHub: https://github.com/jaysomwanshi

---

⭐ If you found this project useful, consider giving it a **Star**!
