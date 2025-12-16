## Week 7 – Security Audit and System Evaluation

In Week 7, I focused on carrying out a security audit on my Ubuntu system to evaluate its overall security posture. This included auditing system configuration, reviewing running services, checking SSH security, and performing basic network security scans. All screenshots and evidence for this week are stored in the `week7-images` folder.

---

### System Update and Preparation
Before starting the audit, I ensured the system was fully up to date. This is important to reduce known vulnerabilities before running any security tools. I used standard update commands and confirmed that pending security updates were identified. Evidence of this step is shown in `update system week 7.png`.

---

### Security Audit with Lynis
I ran a full system security audit using Lynis to assess configuration weaknesses and general system hardening. Lynis checked areas such as kernel settings, file permissions, authentication mechanisms, and logging.

At first, I misunderstood some Lynis options and received an error due to using an invalid flag, but after checking the help output I reran the tool correctly. This helped me understand how auditing tools require accurate syntax.

The successful audit run and output are shown in `run security audit week 7.png`.

---

### Network and SSH Security Assessment
To assess network exposure, I performed a network scan which confirmed the system was reachable and identified active services. I then verified the SSH service configuration using systemd.

Using:
`sudo systemctl status ssh`

I confirmed that the OpenSSH service was active, enabled, and listening on port 22. This allowed me to justify SSH as a required service since it is necessary for remote administration.

During this process, I noticed connection log messages related to closed SSH connections. These were caused by attempted connections being terminated and did not indicate a service failure. This helped me understand how SSH logging works and how to distinguish normal behaviour from actual security issues.

Evidence for this section is provided in:
- `ssh securit & network security scan week7.png`
- `week 7 running services.png`

---

### Running Services Review
As part of the audit, I reviewed active services to ensure that only necessary services were running. The SSH service was identified as active and justified due to its role in secure remote access. No unnecessary services were observed running during this check.

This service verification is shown in `week 7 running services.png`.

---

### Reflection
Week 7 helped me better understand how security auditing works in practice rather than just in theory. I initially struggled with command syntax and interpreting audit output, but resolving these issues improved my confidence in analysing system security. Overall, this week strengthened my understanding of system hardening, service justification, and security evaluation.

All supporting screenshots are available in the `week7-images` folder.

