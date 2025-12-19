# Week 2 – Security Configuration and Firewall Setup

**CMPN202 Operating Systems Coursework**  
**Ilhan Mohamed – A00023555**

---

## 📌 Overview
Week 2 focuses on securing the Ubuntu Server virtual machine by configuring the Uncomplicated Firewall (UFW). The aim was to restrict unauthorised network access while ensuring secure remote administration through SSH.

---

## 1️⃣ Firewall Configuration (UFW)

Before enabling the firewall, SSH access was explicitly allowed to prevent accidental lockout from the server during remote administration.

![Week 2 SSH Allowed](week2-images/week2-ufw-ssh-allowed.png)

Allowing SSH ensures that port 22 remains open so the server can continue to be accessed securely from the Linux Mint workstation.

---

## 2️⃣ Enabling and Verifying Firewall Status

Once SSH access was permitted, the firewall was enabled and its status verified to confirm that the security rules were applied correctly.

![Week 2 UFW Enabled Status](week2-images/week2-ufw-enabled-status.png)

The output confirms that:
- UFW is active and running
- Incoming connections are restricted by default
- SSH traffic is explicitly allowed
- The firewall starts automatically at system boot

---

## 🧠 Reflection
In Week 2, I successfully configured basic network security on the Ubuntu Server using UFW. By enabling the firewall and allowing only essential services such as SSH, the server is protected against unauthorised access while remaining fully manageable remotely. This step is essential in building a secure and controlled operating system environment.
