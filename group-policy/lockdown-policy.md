# Lockdown Policy

## Objective
Create and apply a Group Policy Object (GPO) to restrict standard users from accessing Control Panel and PC Settings.

## Policy Details

| Item | Value |
|---|---|
| Policy Name | `LockDown Policy` |
| Scope | Standard user environment |
| Setting Type | User Configuration |

## Configuration Path
`User Configuration > Administrative Templates > Control Panel`

## Setting Enabled
- **Prohibit access to Control Panel and PC settings**

## Deployment Steps
- Opened **Group Policy Management**
- Created the `LockDown Policy` GPO
- Linked the GPO to the relevant scope in the domain
- Applied updates on the client using:

```cmd
gpupdate /force
```

## Result
Standard users were restricted from opening Control Panel and PC Settings.

## Key Learnings
- Group Policy allows centralized user and device control
- User-based policy settings are useful for standard account lockdown
- Testing after `gpupdate /force` helps confirm deployment success
