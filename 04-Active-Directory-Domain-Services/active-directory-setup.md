# Active Directory Domain Services

## Overview

This section documents the installation and configuration of Active Directory Domain Services (AD DS) on Server01.

Server01 will be configured as the first Domain Controller for the lab environment.

### Lab Domain

```text
adlab.test
```

### Server Information

| Setting | Value |
|---|---|
| Server Name | Server01 |
| Server IP | 192.168.56.10 |
| Operating System | Windows Server |
| Domain | adlab.test |
| Role | Domain Controller |

## Objectives

- Install Active Directory Domain Services.
- Configure Server01 as a Domain Controller.
- Create the `adlab.test` domain.
- Configure DNS as part of the domain controller deployment.
- Verify that Active Directory is functioning correctly.

## Step 1: Installing the Active Directory Domain Services Role

The Active Directory Domain Services role was installed on Server01 using Server Manager.

### Installation Process

1. Opened Server Manager.
2. Selected **Add Roles and Features**.
3. Selected **Role-based or feature-based installation**.
4. Selected Server01 as the destination server.
5. Selected **Active Directory Domain Services**.
6. Added the required features.
7. Reviewed the installation options.
8. Installed the AD DS role.

### Screenshot

![AD DS Role Installed](screenshots/ad-ds-role-installed.png)

### Result

The Active Directory Domain Services role was successfully installed on Server01.

The next step is to promote Server01 to a Domain Controller and create the `adlab.test` domain.
