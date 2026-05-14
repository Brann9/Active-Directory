# Active-Directory IAM Lab
This home lab demonstrates hands-on Identity and Access Management (IAM) using an Active Directory (AD) on RaspberryPi.

It simulates real-world IAM processes including:

- User provisioning (Joiner)
- Role changes (Mover)
- User deprovisioning (Leaver)
- Role based access control (RBAC)
- Access Validation
- File/folder access control

## Environment Setup

Windows 2012 Server domain controller was configured with Active Directory Domain Services (AD DS) and DNS

### Domain Controller Login
<img style="max-width: 100%;" alt="image" src="https://github.com/user-attachments/assets/7feb8d79-8c3e-4313-ab9a-13436758551b" />

### Server Dashboard

<img style="max-width: 100%;" alt="image" src="https://github.com/user-attachments/assets/5a4f2362-1c78-4af8-b683-6a28d9789443" />


## Domain & OU 

A domain (thm.local) was created with Organization Unit (OUs) to reflect different departents:

- IT
- Sales
- Marketing
- Management

### Domain Structure 

<img width="802" height="265" alt="image" src="https://github.com/user-attachments/assets/aa159f26-db5c-4ae6-bc94-0772ae27f33c" />

### OU Structure

<img width="800" height="492" alt="588460710-6d0f208d-6082-4c2c-a6d0-44e0862013b6" src="https://github.com/user-attachments/assets/d57f98e6-55e7-45f4-85ea-310a284be04c" />

## Security Groups (RBAC)

Security groups were created to manage access by role:
- HR_Group
- IT_Admins

### Security Groups

<img width="831" height="530" alt="image" src="https://github.com/user-attachments/assets/49e1aaab-c41a-4ce3-8622-e23e1a08a7d2" />

User Provioning (Joiner)

New users were created and placed into the correct OU based on department

### User Provisioning

<img width="814" height="405" alt="588650178-f5bab6c1-e53a-44e1-adbc-cec10001edbb" src="https://github.com/user-attachments/assets/b98612f2-4fd7-49c2-b513-112725632c03" />

## Role-Based Access Control (RBAC)

Users were assigned to security groups to grant appropriate access.

### User Assigned to Group

<img width="824" height="403" alt="588650376-7928efb4-f751-4495-b172-19cb3dd951bc" src="https://github.com/user-attachments/assets/f3978715-dd63-4359-9f62-c0b623b1c01b" />

## Access Validation (Before Role Change)

### Before Role Change

<img width="817" height="414" alt="588653142-561ed281-3192-47fe-a9b9-e061d6c105e4" src="https://github.com/user-attachments/assets/693bc501-106e-44cc-979a-7776e9d2f0dc" />

## Role Change (Mover)
<img width="842" height="422" alt="image" src="https://github.com/user-attachments/assets/caef7281-d7f9-4fbd-b8e2-2df02d43b9d4" />

## User Deprovisioning (Leaver)

# Account Disabled

## Administrative Access Control

Admin priviledges were assigned via group membership instead of directly to users

# Admin Group Assignment

<img width="699" height="326" alt="589353814-caef7281-d7f9-4fbd-b8e2-2df02d43b9d4" src="https://github.com/user-attachments/assets/37817e80-5bbb-4da7-bb1d-3abe4e76418a" />

## Key IAM Concepts Practiced

- User Lifecycle Management
- Role-Based Access Control (RBAC)
- Least Priviledge Principle
- Access Reviews & Validation
- Security Group Management
- Account Deprovision
- Organizational Unit (OU) Design

## Whats the Purpose of this Project?

This home lab simulates how real organizations manage and identity and access scurely.

It demonstrates the ability to:

- Provision and manage users in Active Directory
- Assign and validate access based on job roles
- Enforce lease priviledge
- Remove access during termination
- Apply access control to resources

## Tools Used
- Active Directory Domain Services (AD DS)
- Windows Server
- VirtualBox
