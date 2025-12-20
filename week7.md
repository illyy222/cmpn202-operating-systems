# Week 7 – Security Audit and System Evaluation

In Week 7, I carried out a security audit on my Ubuntu system to evaluate its overall security posture. This week focused on applying security concepts in practice by reviewing system updates, auditing system configuration, analysing running services, and assessing SSH and network security. The aim was to move beyond theoretical understanding and gain hands-on experience with security auditing and system hardening.

Before starting the audit, I ensured that the system was fully up to date. Keeping the system updated is essential in security, as unpatched systems are more vulnerable to known exploits and weaknesses. I used standard update commands and confirmed that the system was checked for pending updates before running any security tools.

![System update evidence](week7-images/week7-system-update.png)

After updating the system, I ran a full security audit using Lynis to identify configuration weaknesses and potential security issues. The audit assessed areas such as kernel configuration, file permissions, authentication mechanisms, and system logging. Initially, I struggled with Lynis due to incorrect command usage, which resulted in an error. After checking the help output and adjusting the syntax, I was able to rerun the audit successfully. This highlighted how security tools rely heavily on accurate command usage and attention to detail.

![Lynis security audit](week7-images/week7-security-audit.png)

To assess network exposure and remote access security, I reviewed the SSH service configuration using systemd. This confirmed that the OpenSSH service was active, enabled, and listening on port 22. At first, I found it difficult to interpret the SSH output and connection log messages, particularly the closed connection entries. After further investigation, I understood that these messages represented normal behaviour rather than a service failure or security issue, improving my understanding of SSH logging behaviour.

![SSH and network security](week7-images/week7-ssh-network-security.png)

As part of the audit, I reviewed the running services on the system to ensure that only essential services were active. The SSH service was identified as necessary due to its role in secure remote administration. This review helped me understand the importance of service justification and reducing the system’s attack surface to minimise potential security risks.

![Running services](week7-images/week7-running-services.png)

Overall, Week 7 strengthened my understanding of practical security auditing within an operating system environment. Although I faced challenges such as command syntax errors and interpreting audit output, resolving these issues improved my confidence in analysing system security. This week reinforced the importance of system hardening, accurate configuration, and informed decision-making when maintaining a secure operating system.
