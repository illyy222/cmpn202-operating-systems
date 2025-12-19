# Week 4 – User Management and SSH Configuration

**CMPN202 Operating Systems Coursework**  
**Ilhan Mohamed – A00023555**

---

## 📌 Overview

Week 4 focuses on user administration and secure remote access. Tasks included creating a new administrative user, configuring SSH access, and applying firewall rules to improve system security.

---

## 1️⃣ Creating an Administrative User

![Week 4 Create Admin User](week4-images/week4-create-admin-user.png)

A new user account named `studentadmin` was created using the `adduser` command. This user was intended to perform administrative tasks without using the root account directly.

Creating separate admin users improves accountability and security.

---

## 2️⃣ Granting Sudo Privileges

![Week 4 Sudo Privileges](week4-images/week4-sudo-privileges.png)

The `studentadmin` user was added to the sudo group, allowing it to execute administrative commands securely.

This follows best practice by limiting root access while still enabling system administration.

---

## 3️⃣ Enabling SSH Access and Firewall Rules

![Week 4 SSH and UFW](week4-images/week4-ssh-ufw.png)

SSH was enabled to allow remote access to the server. Firewall rules were configured using UFW to permit SSH connections while maintaining network security.

This ensures secure remote management of the server.

---

## 🧠 Reflection

I initially struggled with understanding how user permissions and sudo access worked together. After testing commands and switching between users, I gained a clearer understanding of Linux privilege separation.

This week helped me understand the importance of secure user management and controlled remote access.
