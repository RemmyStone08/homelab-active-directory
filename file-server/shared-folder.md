\# File Server - Shared Folder Setup



\## Objective

Create a shared folder on the Windows Server and make it accessible to domain users from a domain-joined client machine.



\## Folder Created

\- `C:\\CompanyFiles`



\## Share Configuration

\- Enabled Advanced Sharing

\- Shared folder name: `CompanyFiles`



\## Share Permissions

\- Added: `Domain Users`

\- Allowed:

&#x20; - Read

&#x20; - Change



\## NTFS Permissions

On the Security tab:

\- Added: `Domain Users`

\- Allowed:

&#x20; - Modify

&#x20; - Read \& Execute

&#x20; - List folder contents

&#x20; - Read

&#x20; - Write



\## Client Access Test

From the Windows 10 domain-joined client:

\- Opened `\\\\dc01`

\- Opened the `CompanyFiles` share

\- Successfully accessed the folder as a domain user



\## Drive Mapping

Mapped the share as a network drive on the client machine.



Example path:

`\\\\dc01\\CompanyFiles`



\## Key Learning

This demonstrated the difference between:

\- Share permissions

\- NTFS permissions



It also showed how centralized file access works in a domain environment.

