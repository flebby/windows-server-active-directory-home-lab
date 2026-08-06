# Windows Server 2022 Installation

## Project Objective

The objective of this phase was to create a Windows Server 2022 virtual machine using Oracle VirtualBox and prepare it for Active Directory and system administration tasks.

---

## Lab Environment

| Component | Details |
|-----------|---------|
| Host Operating System | Windows 10/11 |
| Virtualization Software | Oracle VirtualBox |
| Guest Operating System | Windows Server 2022 Evaluation |
| Virtual Machine Name | Server01 |

---

## Virtual Machine Configuration

| Setting | Value |
|---------|-------|
| Name | Server01 |
| Operating System | Windows Server 2022 (64-bit) *(Windows 2019 (64-bit) selected in VirtualBox if 2022 was unavailable)* |
| Memory | 4096 MB (4 GB) |
| Processor | 2 CPU Cores |
| Hard Disk | 60 GB (Dynamically Allocated VDI) |
| Network Adapter | NAT |

---

## Installation Steps

1. Opened Oracle VirtualBox.
2. Created a new virtual machine named **Server01**.
3. Allocated 4 GB of RAM and 2 CPU cores.
4. Created a 60 GB dynamically allocated virtual hard disk.
5. Configured the network adapter to use NAT.
6. Attempted to start the virtual machine.

---

## Issue Encountered

When starting the virtual machine, the following error was displayed:

> **FATAL: No bootable medium found! System halted.**

### Cause

The Windows Server 2022 ISO image had not yet been attached to the virtual machine, so VirtualBox could not find a bootable operating system.

### Resolution

1. Powered off the virtual machine.
2. Opened **Settings > Storage** in VirtualBox.
3. Selected the virtual optical drive.
4. Attached the Windows Server 2022 Evaluation ISO.
5. Saved the settings.
6. Restarted the virtual machine.

After attaching the ISO, the Windows Server installation could begin successfully.

---

## Screenshots

### Virtual Machine Created

![Server01-Created](screenshots/server01-created.png)

### Boot Error

![No Bootable Medium Error](screenshots/no-bootable-medium.png)

### Windows Server ISO Attached

![ISO Mounted](screenshots/windows-server-iso-mounted.png)

---

## Skills Demonstrated

- Virtual machine creation
- VirtualBox configuration
- Windows Server deployment
- Boot troubleshooting
- Virtual storage configuration

---

## Lessons Learned

A virtual machine requires a bootable installation media before an operating system can be installed. If no ISO is attached, VirtualBox displays the message **"No bootable medium found! System halted."** Attaching the Windows Server ISO through the Storage settings resolves the issue.

---

## Next Steps

- Install Windows Server 2022.
- Configure the Administrator account.
- Rename the server.
- Configure a static IP address.
- Install Active Directory Domain Services.
