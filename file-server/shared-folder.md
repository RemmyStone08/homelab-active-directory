# Shared Folder Setup

## Objective
Create a shared folder on the Windows Server and make it accessible to domain users from a domain-joined client machine.

## Folder Details

| Item | Value |
|---|---|
| Local Path | `C:\CompanyFiles` |
| Share Name | `CompanyFiles` |
| Access Path | `\\dc01\CompanyFiles` |

## Share Configuration
- Enabled **Advanced Sharing**
- Shared the folder as `CompanyFiles`

## Share Permissions
Added `Domain Users` with:
- Read
- Change

## NTFS Permissions
Added `Domain Users` with:
- Modify
- Read & Execute
- List folder contents
- Read
- Write

## Client Access Test
From a Windows 10 domain-joined client:
- Opened `\\dc01`
- Accessed the `CompanyFiles` share
- Confirmed successful access as a domain user

## Drive Mapping
The shared folder was mapped as a network drive on the client machine for easier access.

## Key Learnings
- Share permissions and NTFS permissions work together
- Centralized file access is easier to manage in a domain environment
- Testing from the client side is important to confirm permission behavior
