# Week 1 – System Planning and Distribution Selection  
**CMPN202 Operating Systems Coursework**  
**Ilhan Mohamed – A00023555**

## 📌 Overview  
Week 1 focuses on planning the dual VirtualBox setup, choosing an appropriate server OS, configuring the workstation environment, and collecting the initial technical specifications of both systems.


# 1️⃣ System Architecture Diagram  
![Week 1 System Architecture Diagram](week%201%20OS%20diagram.png)

This shows how my Linux Mint workstation VM connects to my Ubuntu Server 22.04 VM using a VirtualBox Host-Only Network.

---

# 2️⃣ Distribution Selection Justification  
**Chosen Server Distribution:** Ubuntu Server 22.04 LTS (Headless)

### ✔ Why I chose Ubuntu Server:
- Long-term support  
- Strong documentation  
- Perfect for SSH-only administration  
- Lightweight and reliable in VirtualBox  
- Comes with UFW + AppArmor  

### Alternatives considered:
Debian Server, Rocky Linux, AlmaLinux, CentOS Stream.

---

# 3️⃣ Workstation Configuration Decision  
**Workstation Used:** Linux Mint Desktop VM  

### ✔ Why Mint?
- Full GUI  
- Easy SSH access  
- Helps with monitoring + scripting  
- Matches the dual-system architecture

---

# 4️⃣ Network Configuration Documentation  

### VirtualBox Networking Mode  
I used a **Host-Only Network**, which allows the two VMs to communicate securely without internet exposure.

### Network Summary  
| System | IP Address | Interface | Purpose |
|--------|------------|-----------|---------|
| Ubuntu Server | *Shown in screenshot below* | enp0s3 | Receives SSH connections |
| Mint Workstation | *Shown in screenshot below* | Host-Only Adapter | Administers the server |

### VirtualBox Settings Evidence  
*(IP proof is shown in my screenshots in the next section.)*

---

# 5️⃣ System Specification Evidence  
These commands were run on the **Ubuntu Server** VM to document its system specifications:

- `uname -a`  
- `free -h`  
- `df -h`  
- `ip addr`  
- `lsb_release -a`  

### 📸 Combined Screenshot Evidence  
Since I ran all commands during one session, all outputs are visible in the screenshot below:

![Ubuntu System Specs](Screenshot%202025-12-02%20160825.png)

### 📸 Network Communication Evidence  
This screenshot shows both VMs running side-by-side, including both IP addresses:

![VM Network Evidence](Screenshot%202025-12-02%20161140.png)

---
