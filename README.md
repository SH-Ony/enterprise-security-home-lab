# Enterprise Security Home Lab

## Overview

This repository documents my journey of building a realistic enterprise security home lab from scratch.

The objective is not only to configure virtual machines, but to understand how enterprise infrastructure is designed, secured, monitored, and administered.

The lab is built entirely in VirtualBox and simulates a small enterprise network consisting of Windows and Linux systems protected by a pfSense firewall.

---

# Objectives

- Build an enterprise network from scratch
- Learn Windows Server Administration
- Deploy Active Directory Domain Services
- Understand DNS and DHCP
- Practice Identity and Access Management
- Administer Linux servers
- Configure pfSense Firewall
- Implement security hardening
- Simulate real-world attacks
- Practice detection and incident response

---

# Current Lab Components

| Component | Purpose |
|------------|----------|
| pfSense Community Edition | Firewall, Router, Gateway |
| Windows Server 2022 | Domain Controller (DC01) |
| Windows 10 | Enterprise Client |
| Ubuntu Desktop | Linux Workstation |
| Ubuntu Server | Linux Server |

---
```text
Internet
   |
VirtualBox NAT
   |
pfSense
   |
10.10.20.0/24 Internal Network
   |
+----------------+----------------+----------------+----------------+
|                |                |                |
DC01             Windows 10       Ubuntu Desktop   Ubuntu Server
10.10.20.10      DHCP             DHCP             DHCP
```
---

# Planned Technologies

- Active Directory
- DNS
- DHCP
- Group Policy
- LDAP
- Kerberos
- Windows Administration
- Linux Administration
- pfSense
- SSH
- Docker
- Wazuh SIEM
- Sysmon
- Zeek
- Security Onion (future)
- Kali Linux
- Vulnerability Assessment
- Threat Detection

---

# Learning Philosophy

Every configuration performed in this lab is documented with:

- Objectives
- Configuration steps
- Network diagrams
- Screenshots
- Problems encountered
- Troubleshooting
- Lessons learned

The goal is to understand **why** every configuration is required rather than simply following tutorials.

---

# Progress

- ✅ Module 1 — Enterprise Network Foundation
- ⏳ Module 2 — Active Directory
- ⏳ Module 3 — Domain Joined Clients
- ⏳ Module 4 — Linux Administration
- ⏳ Module 5 — Security Hardening
- ⏳ Module 6 — Identity & Access Management
- ⏳ Module 7 — Monitoring & Logging
- ⏳ Module 8 — Attack Simulation
