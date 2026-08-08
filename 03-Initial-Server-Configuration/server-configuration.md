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
