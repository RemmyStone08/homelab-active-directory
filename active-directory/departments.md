\# Active Directory - Departments and Access Control



\## Objective

Organize users into departments and control access to resources using Active Directory.



\## Departments Created

\- IT

\- HR

\- Sales



\## Organizational Units (OUs)

Created separate OUs for each department:

\- IT OU

\- HR OU

\- Sales OU



\## Users

Created users and assigned them to departments:

\- John → IT

\- Sarah → HR

\- (Add your actual users if different)



\## Group Strategy

Used a basic Role-Based Access Control (RBAC) model:



\- Created security groups per department:

&#x20; - IT\_Group

&#x20; - HR\_Group

&#x20; - Sales\_Group



\- Added users to their respective groups



\## Access Control

Configured folder permissions so that:

\- IT users can access IT resources

\- HR users can access HR resources

\- Sales users can access Sales resources



\## Testing

\- Logged in as different users

\- Verified access is restricted based on department

\- Confirmed users cannot access other departments’ data



\## Key Learning

\- How to structure users using OUs

\- Importance of security groups

\- Basic implementation of RBAC (Role-Based Access Control)

\- Separation of access based on job role

