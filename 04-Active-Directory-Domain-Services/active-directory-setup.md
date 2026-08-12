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
