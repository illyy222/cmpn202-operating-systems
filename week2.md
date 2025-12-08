# Week 2 – Security Configuration and Firewall Setup (Ubuntu)

## Objective
The objective of Week 2 was to secure the Ubuntu virtual machine by:
- Updating the system
- Installing and configuring the firewall (UFW)
- Allowing secure SSH access
- Verifying firewall status

---

## System Update
The system was first updated to ensure all packages were up to date before applying security settings.

Command used:
sudo apt update

This ensures the latest security patches and package versions are available.

(See screenshot: week2-apt-update.png)

---

## Installing UFW Firewall
UFW (Uncomplicated Firewall) was installed to manage network traffic securely.

Command used:
sudo apt install ufw -y

UFW was already installed but verified to be the latest version.

(See screenshot: week2-ufw-install.png)

---

## Checking Firewall Status
Before enabling the firewall, its status was checked.

Command used:
sudo ufw status verbose

The firewall was initially inactive.

(See screenshot: week2-ufw-status-inactive.png)

---

## Allowing SSH Access
SSH access was allowed to prevent remote lockout when enabling the firewall.

Command used:
sudo ufw allow ssh

This opened port 22 for secure remote connections.

---

## Enabling the Firewall
The firewall was then enabled.

Command used:
sudo ufw enable

The firewall became active and started automatically at system startup.

---

## Final Firewall Verification
The firewall status was checked again to confirm the configuration.

Command used:
sudo ufw status verbose

Results:
- Firewall status: Active
- Default policy: Deny incoming, Allow outgoing
- SSH (port 22) allowed

(See screenshot: week2-ufw-status-active.png)

---

## Reflection
In Week 2, I successfully secured the Ubuntu virtual machine by configuring the firewall using UFW. This ensures protection against unauthorised access while allowing secure SSH connections. This is an essential step in building a secure operating system environment.
