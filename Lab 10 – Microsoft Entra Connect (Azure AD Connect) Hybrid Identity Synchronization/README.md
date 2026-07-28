# Microsoft Entra Connect (Azure AD Connect) Hybrid Identity Synchronization Lab

![Azure](https://img.shields.io/badge/Microsoft-Azure-0078D4?style=for-the-badge\&logo=microsoftazure)
![Identity](https://img.shields.io/badge/Identity-Microsoft%20Entra%20ID-blue?style=for-the-badge)
![Hybrid Identity](https://img.shields.io/badge/Hybrid-Identity-success?style=for-the-badge)

## Lab Overview

This lab demonstrates configuring **Microsoft Entra Connect Sync** to synchronize identities between an on-premises **Active Directory Domain Services (AD DS)** environment and **Microsoft Entra ID**.

The objective is to build a hybrid identity environment where users can use the same identity across on-premises and cloud services.

---

## Architecture

```text
On-Premises Active Directory Domain Services
                 |
                 |
      Microsoft Entra Connect Sync
                 |
                 |
          Microsoft Entra ID Tenant
                 |
                 |
       Microsoft 365 / Azure Services
```

---

## Objectives

* Install Microsoft Entra Connect Sync
* Configure synchronization between AD DS and Microsoft Entra ID
* Connect on-premises Active Directory
* Configure sign-in settings
* Validate synchronization configuration
* Understand hybrid identity architecture

---

## Prerequisites

* Azure Subscription
* Microsoft Entra ID Tenant
* Global Administrator account
* Windows Server with Active Directory Domain Services
* Domain Administrator credentials
* Microsoft Entra Connect Sync installer

---

# Implementation Steps

## 1. Verify Microsoft Entra Admin Center Access

Verified Microsoft Entra Admin Center access using Global Administrator account.

![Microsoft Entra Admin Center Overview](screenshots/02-browser-microsoft-entra-admin-global-admin-overview.png)

---

## 2. Microsoft Entra Connect Download

Searched and downloaded Microsoft Entra Connect Sync agent.

![Microsoft Entra Connect Search](screenshots/03-microsoft-entra-connect-search.png)

![Microsoft Entra Connect Download](screenshots/04-microsoft-entra-connect-overview-download.png)

![Terms and Agreement](screenshots/05-Download-connect-sycn-agent-terms-and-agreement.png)

---

## 3. Install Microsoft Entra Connect

Accepted license agreement and started Microsoft Entra Connect installation.

![Microsoft Entra Connect Installation](screenshots/06-welcome-to-microsoft-entra-connect-i-agree-install.png)

---

## 4. Configure Express Settings

Selected Express Settings for initial synchronization configuration.

![Express Settings](screenshots/07-express-settings.png)

---

## 5. Connect Microsoft Entra ID

Signed in using Global Administrator credentials.

![Microsoft Entra Sign In](screenshots/08-sign-in.png)

---

## 6. Connect Active Directory Domain Services

Configured connection with on-premises Active Directory Domain Services.

![Connect Active Directory](screenshots/09-connect-to-adds-user-password-ad.png)

---

## 7. Configure Sign-In Configuration

Configured Microsoft Entra ID sign-in options.

![Sign-In Configuration](screenshots/10-microsoft-entra-sign-in-configuration.png)

---

## 8. Synchronization Configuration

Completed Microsoft Entra Connect synchronization configuration.

![Configuration Progress](screenshots/11-configuring-screen.png)

![Configuration Complete](screenshots/12-configuration-complete.png)

---

# Verification

Completed validation checks:

* Microsoft Entra Connect installed successfully
* Active Directory connector configured
* Synchronization configuration completed
* Hybrid identity environment prepared

---

# Commands Used

```powershell
whoami
hostname
ipconfig /all
systeminfo
```

Command verification screenshot:

![Commands Used](screenshots/01-cmd-commands-used.png)

---

# Skills Demonstrated

* Microsoft Entra ID
* Hybrid Identity
* Active Directory Domain Services
* Identity Synchronization
* Microsoft Entra Connect Sync
* Cloud Identity Management
* Enterprise Authentication

---

# Lab Status

✅ Completed
