# 🚀 Linux Security Hardening & Audit Lab
*Implementing security guidelines and compliance on Linux servers (Ubuntu).*

- Objective
```text
This lab demonstrates the application of Hardening techniques to reduce the attack surface.
Using the Lynis professional audit tool, I successfully increased the security index from 63 to 70.
```

- Environment
```
OS: Ubuntu Server 22.04 LTS
Virtualization: VMware / VirtualBox
Audit Tools: Lynis, Auditd
Network Security: UFW (Uncomplicated Firewall)
```

- Technical Implementations
```
1. Access Control & SSH
- Custom SSH Port: Changed default port 22 to 2222.
- Key-Based Auth: Enforced Ed25519 cryptographic keys.
- Root Login: Disabled direct root access.
- Legal Banner: Implemented compliance warning via /etc/issue.net.
```
2. Network Security
```
- Policy: Configured UFW with "Default Deny" incoming policy.
- Rules: Allowed only specific traffic on port 2222/TCP.
```
- Results & Evidence

Firewall Status & Listening Ports

<img width="566" height="206" alt="image" src="https://github.com/user-attachments/assets/fabb15d9-79f5-4ee3-b493-c6f5a2d8c51a" />

Final Hardening Index (70)

<img width="978" height="602" alt="image" src="https://github.com/user-attachments/assets/8258799b-3af3-4488-b8b2-7db79848bb99" />

- Conclusion
```
Reaching a Hardening Index of 70 represents a system with compliance levels above market average.
This lab strikes a balance between maximum security and operational usability.
This project demonstrates proficiency in Blue Team systems administration and technical compliance.
```
