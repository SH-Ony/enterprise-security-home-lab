
# Module 1 — Enterprise Network Foundation

## Objective

The objective of this module was to build the foundation of a small enterprise-style virtual network using VirtualBox, pfSense, Windows, and Ubuntu systems.

This module focused on understanding and configuring:

- Virtual networking
- IP addressing
- Subnet masks
- Default gateways
- DHCP
- DNS basics
- Routing
- Firewall rules
- Connectivity testing
- Basic troubleshooting

---

## Lab Components

| Machine | Role | Network |
|---|---|---|
| pfSense | Firewall, router, gateway | WAN + Internal LAN |
| Windows Server 2022 | Future Domain Controller | 10.10.20.10 |
| Windows 10 | Enterprise client | DHCP |
| Ubuntu Desktop | Linux workstation | DHCP |
| Ubuntu Server | Linux server | DHCP |

---

## Network Design

```text
Internet
   |
VirtualBox NAT
   |
pfSense WAN
   |
pfSense Internal Interface
10.10.20.254
   |
10.10.20.0/24 Internal Network
   |
+----------------+----------------+----------------+----------------+
|                |                |                |
DC01             Windows 10       Ubuntu Desktop   Ubuntu Server
10.10.20.10      DHCP             DHCP             DHCP
