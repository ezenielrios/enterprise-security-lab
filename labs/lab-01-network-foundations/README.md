# Lab 01 – Network & Firewall Foundations (pfSense)

## Overview

This lab establishes the foundational network security architecture for the enterprise security lab. A pfSense firewall is deployed as the primary network boundary device, providing routing, segmentation, and management access for subsequent offensive and defensive security testing.

The objective of this lab is **infrastructure correctness**, not exploitation.

---

## Objectives

- Deploy pfSense in a virtualized environment  
- Configure WAN and LAN interfaces correctly  
- Establish secure management access  
- Validate network connectivity and routing  
- Prepare the environment for future attack, detection, and response labs  

---

## Environment

| Component        | Details                     |
|------------------|-----------------------------|
| Hypervisor       | VMware Workstation          |
| Firewall         | pfSense CE 2.7.2            |
| WAN Interface    | NAT (VMnet8)                |
| LAN Interface    | Host-Only (VMnet1)          |
| LAN Subnet       | `192.168.59.0/24`           |
| Firewall IP      | `192.168.59.1`              |

---

## Network Topology
[ Internet ]
|
(NAT)
|
[ pfSense WAN ]
[ pfSense LAN ] ─── 192.168.59.0/24 ─── [ Security VMs ]

---

## Installation Summary

- pfSense CE installed via ISO  
- Guided disk setup used  
- Interfaces manually assigned:
  - `em0` → WAN  
  - `em1` → LAN  
- DHCP enabled on LAN  
- WebConfigurator accessed via HTTPS  

---

## Validation Steps

- pfSense console confirms interface assignments  
- WebConfigurator reachable at:

https://192.168.59.1

- Firewall services confirmed listening on port 443  
- LAN DHCP range functioning correctly  

---

## Security Notes

- Default admin credentials identified and flagged  
- Self-signed TLS certificate acknowledged  
- Password change scheduled for follow-up hardening lab  

---

## Outcome

A functional and stable firewall perimeter is now in place. This environment serves as the baseline for all future labs, including vulnerability scanning, intrusion detection, exploitation testing, and incident response scenarios.

---

## Next Lab

**Lab 02 – Network Scanning & Enumeration**

- Nmap discovery  
- Service fingerprinting  
- Baseline asset visibility  

---

## Disclaimer

This lab is conducted in an isolated environment for educational and defensive security research purposes only.

