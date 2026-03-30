# Departments and Access Control

## Objective
Organize users into departments and control access to resources using Active Directory.

## Departments Created
- IT
- HR
- Sales

## Organizational Units (OUs)
Separate OUs were created for each department:
- `IT`
- `HR`
- `Sales`

## Users
Example users were created and assigned to departments:
- John → IT
- Sarah → HR
- Sales user → Sales

## Group Strategy
A basic Role-Based Access Control (RBAC) approach was used.

### Security Groups
- `IT_Group`
- `HR_Group`
- `Sales_Group`

### Assignment Process
- Users were added to the group that matched their department
- Permissions were assigned to groups instead of directly to users

## Access Control
Folder permissions were configured so that:
- IT users could access IT resources
- HR users could access HR resources
- Sales users could access Sales resources

## Testing
- Signed in as different users
- Verified that access matched each department
- Confirmed users could not access data outside their own department

## Key Learnings
- OUs help organize domain objects clearly
- Security groups simplify permission management
- RBAC makes access easier to scale and maintain
