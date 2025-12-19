# Week 4 – User Management and Privilege Control

CMPN202 Operating Systems Coursework  
Ilhan Mohamed – A00023555

---

## 📌 Overview

Week 4 focuses on **user account management and privilege control** on the Ubuntu Server.  
The aim was to understand how Linux separates standard users from administrative users, how elevated privileges are granted securely using `sudo`, and how access can be verified to reduce the risk of unauthorised system changes.

---

## 1️⃣ Creating an Administrative User

![Week 4 Create Admin User](week4-images/create-admin-user.png)

A new user account (`studentadmin`) was created using the `adduser` command.  
This ensures administrative tasks are not performed using the root account, improving system security and accountability.

Key points:
- Separate user accounts reduce risk
- Each user has isolated permissions
- Follows best practice for Linux administration

---

## 2️⃣ Adding User to the Sudo Group

![Week 4 Add User to Sudo Group](week4-images/add-user-to-sudo-group.png)

The newly created user was added to the `sudo` group, granting controlled administrative privileges.  
This allows the user to execute system-level commands when required, without giving unrestricted root access.

Command used:
```bash
sudo usermod -aG sudo studentadmin
