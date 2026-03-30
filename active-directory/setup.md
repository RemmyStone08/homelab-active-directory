# Active Directory Setup

## Objective
Set up a Windows Server 2019 domain controller and configure Active Directory Domain Services for a lab environment.

## Server Details

| Item | Value |
|---|---|
| Hostname | `DC01` |
| Server OS | Windows Server 2019 |
| Domain | `remmy.local` |
| Platform | VirtualBox |

## Steps Performed

### 1. Installed Windows Server 2019
- Installed the operating system in VirtualBox
- Assigned a static IP address
- Confirmed basic network connectivity

### 2. Installed Active Directory Domain Services
- Opened **Server Manager**
- Added the **Active Directory Domain Services** role
- Completed the required installation steps

### 3. Promoted the Server to a Domain Controller
- Created a new forest: `remmy.local`
- Set the Directory Services Restore Mode (DSRM) password
- Completed domain controller promotion
- Rebooted the server

### 4. Verified the Deployment
- Confirmed domain functionality after restart
- Opened **Active Directory Users and Computers**
- Verified the initial domain structure

## Result
A working Windows Server domain controller was successfully deployed and configured for the lab.

## Key Learnings
- DNS is critical in domain environments
- AD DS provides centralized identity and access management
- Promoting a domain controller requires careful planning around naming and networking
