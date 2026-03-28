Group Policy - User Restriction Policy



\# Objective

Create and apply a Group Policy Object to restrict standard users from accessing Control Panel and PC Settings.



\# Policy Created

\- \*\*Policy Name:\*\* LockDown Policy



\# Configuration

Path used:

`User Configuration > Administrative Templates > Control Panel`



Setting enabled:

\- \*\*Prohibit access to Control Panel and PC settings\*\*



\# Deployment

\- Created the GPO in Group Policy Management

\- Linked the policy to the relevant scope in the domain

\- Applied policy updates on the client machine using:



```cmd

gpupdate /force

