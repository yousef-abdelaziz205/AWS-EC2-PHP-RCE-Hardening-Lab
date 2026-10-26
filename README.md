# AWS-EC2-PHP-RCE-Hardening-Lab
# AWS EC2 PHP RCE & Server Hardening Lab 🚀

Hands-on lab demonstrating vulnerability simulation (PHP Remote Code Execution) and server hardening best practices on an AWS EC2 Ubuntu instance, completed as part of the Digital Egypt Pioneers Initiative (DEPI) - AWS Cloud Security Track.

---

## 🛠️ Lab Architecture & Environment
- **Cloud Provider:** Amazon Web Services (AWS)
- **Compute:** EC2 Instance (`t3.micro`) running Ubuntu & Apache2 Web Server.
- **Security Focus:** Vulnerability Remediation, Access Controls, and Defense-in-Depth.

---

## 📋 Implementation Steps

### 1. Environment Deployment
- Launched an EC2 Ubuntu instance on AWS.
- Configured security groups and initialized the Apache2 web server to host the local test environment.

### 2. Vulnerability Simulation (The Exploit)
- Deployed a PHP-based Remote Code Execution (RCE) Proof of Concept (PoC) to simulate real-world web application vulnerabilities.
- Verified successful command execution and server response (`200 OK`) via the test script.

### 3. Server Hardening & Remediation
To secure the server and mitigate risks, the following hardening steps were implemented:
- **PHP Hardening:** Modified `php.ini` settings (e.g., disabling dangerous functions like `exec`, `shell_exec`, and hiding PHP version details).
- **File Permissions & Ownership:** Enforced strict file permissions on web directories to prevent unauthorized modifications by the web server user (`www-data`).
- **Firewall Configuration (UFW):** Configured Uncomplicated Firewall to restrict incoming traffic and allow only necessary ports (HTTP/HTTPS/SSH).
- **Log Monitoring:** Enabled and reviewed system and web server logs to track access patterns and anomalies.

---

## 👤 Author
- **Yousef Abdelaziz**
- **Track:** AWS Cloud Security | DEPI
