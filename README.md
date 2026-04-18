 Linux Security Hardening & Audit Lab
 
Implementing security guidelines and compliance on Linux servers (Ubuntu).

    Objective
    This lab demonstrates the application of Hardening techniques to reduce the attack surface of a Linux server. 
    Using the Lynis professional audit tool, I successfully increased the security index from 63 to 70. The project focuses on system integrity, rigorous access control, and active monitoring.


    Environment
    OS: Ubuntu Server 22.04 LTS 
    Virtualization: VMware / VirtualBox
    Audit Tools: Lynis, Auditd 
    Network Security: UFW (Uncomplicated Firewall) 

Technical Implementations (The Hardening Process)

1. Access Control & SSH Hardening
Custom SSH Port: Changed the default port (22 to 2222) to mitigate automated brute-force attacks.
Key-Based Authentication: Disabled password authentication, enforcing the use of Ed25519 cryptographic keys.
Root Login Restriction: Prohibited direct root login to ensure the principle of least privilege.
Legal Banner: Implemented a pre-login compliance warning (/etc/issue.net) for audit requirements.

2. Network Security (Firewall)
Restrictive Policy: Configured UFW with a "Default Deny" incoming policy.

Granular Rules: Only allowed incoming traffic on the custom administration port (2222/TCP).

3. Auditing and Monitoring
System Auditing: Installed and configured Auditd to track critical kernel events and file changes.

Vulnerability Scanning: Utilized Lynis for automated security auditing and identification of configuration flaws.

4. Kernel Hardening (Sysctl)
Networking Security: Applied sysctl tweaks to prevent IP Spoofing and ignore malicious ICMP redirects.

Results & Evidence
Firewall Status & Listening Ports:
Showcasing the active UFW and the service listening on the custom port.
<img width="566" height="206" alt="image" src="https://github.com/user-attachments/assets/23fc5ec4-7327-4f81-bb74-d60e07ab0204" />

Final Hardening Index (70):
Final audit report proving the security improvements.
<img width="978" height="602" alt="image" src="https://github.com/user-attachments/assets/9d108060-cf77-4b15-b195-3e99c479136b" />

Conclusion
Reaching a Hardening Index of 70 represents a system with compliance levels above market average. This lab strikes a balance between maximum security and operational usability. This project demonstrates proficiency in Blue Team systems administration and technical compliance.
