# Initial Windows Server Configuration

## Overview

This section documents the initial configuration of the Windows Server virtual machine before deploying Active Directory Domain Services.

The server will be used as the primary server for the Active Directory home lab.

## Server Information

| Configuration | Value |
|---|---|
| Server Name | Server01 |
| Operating System | Windows Server |
| Virtualization Platform | Oracle VirtualBox |
| Purpose | Active Directory Domain Controller |

---

## Step 1: Rename the Server

The Windows Server computer name was configured as:

```text
Server01
```

A descriptive server name makes it easier to identify the server when managing multiple systems in a network.

### Screenshot

![Server01 Renamed](screenshots/server01-renamed.png)

---

## Result

The server was successfully renamed to `Server01` and restarted to apply the change.

## Next Step

The next step is to configure a static IP address for Server01.

## Step 2: Reviewing Current Network Configuration

Before assigning a static IP address, the existing network configuration was reviewed.

The server was initially configured to obtain its network settings automatically through DHCP.

### Current Configuration

| Setting | Value |
|---|---|
| DHCP | Enabled |
| IPv4 Address | 10.0.2.15 |
| Subnet Mask | 255.255.255.0 |
| Default Gateway | 10.0.2.2 |
| DHCP Server | 10.0.2.2 |
| DNS Server | 172.20.10.1 |

### Why This Matters

A server used for Active Directory should have a predictable IP address. Dynamic addressing can cause the server's IP address to change, which can create problems for services that depend on a consistent address.

The next step will be to configure a static IP address for Server01.

### Screenshot

![Server01 Network Configuration](screenshots/server01-network-details.png)
