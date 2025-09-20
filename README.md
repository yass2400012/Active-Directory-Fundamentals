# Active Directory Fundamentals (TryHackMe Lab)

This project documents my hands-on work in **TryHackMe Cyber Security 101** and **Windows & Active Directory Fundamentals** labs.  
The focus was on learning how to configure and manage **Active Directory (AD DS)**, apply **Group Policy Objects (GPOs)**, manage **users, machines, groups, and OUs**, and simulate real-world IT administration tasks in a Windows domain environment.

<br>

![Active Directory OU Structure](project-screenshots/OU_Structure.PNG)

---

# Lab Checklist

# Part 1: Active Directory Basics

### Core Concepts
- **AD DS** acts as a catalogue that holds all network objects (users, groups, machines, printers, shares).
- **Security Principals** (users, groups, machines) can be authenticated and assigned privileges.

📸 Example: Viewing AD DS in the Domain Controller  
![Active Directory Basics](project-screenshots/AD_Basics.PNG)

---

# Part 2: User & Machine Accounts

### Users
- Represent employees or services.
- Can be authenticated and assigned permissions.

### Machines
- Each domain-joined machine creates a machine account (e.g., `DC01$`).
- Passwords are long (120 characters) and auto-rotated.

📸 Example: Adding users in ADUC  
![User Creation Screenshot](project-screenshots/User_Creation.PNG)

---

# Part 3: Security Groups

- Groups simplify access management by granting privileges to multiple users/machines at once.
- Examples:
  - **Domain Admins** – Admin privileges across domain.
  - **Backup Operators** – Can access files for backup.
  - **Domain Users** – All domain users.
  - **Domain Computers** – All domain machines.

📸 Example: Security groups in AD  
![Security Groups Screenshot](project-screenshots/Security_Groups.PNG)

---

# Part 4: Organizational Units (OUs)

- OUs organize users/computers into logical structures.
- Used for applying **Group Policy Objects (GPOs)**.
- Example structure created:
  - IT
  - Marketing
  - Sales
  - Management
  - R&D
  - Students (custom)

📸 Example: OU Structure in AD  
![OU Screenshot](project-screenshots/OU_Structure.PNG)

---

# Part 5: Delegation of Control

- Delegation allows junior IT staff to perform tasks without domain admin rights.
- Example: Allowing "Phillip" (IT Support) to reset user passwords in Sales OU.

📸 Example: Delegating password reset rights  
![Delegation Screenshot](project-screenshots/Delegation.PNG)

---

# Part 6: Group Policy Objects (GPOs)

- **GPOs** apply configurations and security baselines.
- Examples implemented:
  - Restrict non-IT users from accessing **Control Panel**.
  - Auto-lock workstations after **5 minutes** of inactivity.

📸 Example: GPO configuration in Group Policy Management  
![GPO Screenshot](project-screenshots/GPO_Config.PNG)

---

# Skills Demonstrated

| Tools & Technologies             | Description                                        |
| -------------------------------- | -------------------------------------------------- |
| Active Directory Domain Services | Managing users, groups, and machines               |
| Group Policy Objects (GPOs)      | Applying domain-wide policies and baselines        |
| Windows Server (DC)              | Domain Controller setup and administration         |
| PowerShell                       | Used for user management and password resets       |
| Event Viewer                     | Log inspection and troubleshooting                 |
| Organizational Units (OUs)       | Logical structuring of AD objects                  |

<br>

| Security & IT Skills          | Description                                    |
| ----------------------------- | ---------------------------------------------- |
| Identity & Access Management  | Managing users, groups, and permissions        |
| Policy Enforcement            | Enforcing security baselines via GPOs          |
| Account Delegation            | Delegating control for IT support              |
| Log Monitoring                | Using Event Viewer to track AD activity        |
| Network Administration        | Understanding AD structure and domain objects  |

---

# Final Result

✔ Configured and managed Active Directory Domain Services (AD DS)  
✔ Created and managed **users, groups, and machine accounts**  
✔ Designed and implemented **OU structures**  
✔ Applied **GPOs** for security and user restrictions  
✔ Practiced **delegation of privileges** for IT support staff  
✔ Strengthened understanding of **enterprise identity and access management**


