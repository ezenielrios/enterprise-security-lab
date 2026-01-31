# Enterprise Security Lab

## Overview

This repository documents the design and implementation of an enterprise-style information security lab built using free and open-source tools. The lab simulates real-world security operations across networking, detection, vulnerability management, adversary simulation, and incident response.

The focus is on **professional security workflows**, not CTF-style challenges.

This project is designed to reflect how security teams operate in production environments: building infrastructure first, validating visibility, then layering testing, monitoring, and response capabilities.

---

## Goals

- Build a realistic enterprise security lab from the ground up  
- Practice defensive and offensive security workflows end-to-end  
- Document methodology, tooling, and decision-making clearly  
- Demonstrate hands-on capability aligned with security engineering roles  

---

## Lab Structure

enterprise-security-lab/
│
├── labs/ # Step-by-step lab exercises
├── evidence/ # Screenshots, logs, sanitized outputs
├── docs/ # Architecture notes and design documentation
└── README.md # Project overview (this file)

---

## Technologies Used

- pfSense (network perimeter & routing)
- VMware Workstation
- Linux security tooling (Nmap, OpenVAS, Burp Suite, etc.)
- Dockerized vulnerable applications
- Log analysis and traffic inspection tools

> All tooling is deployed in isolated, controlled environments.

---

## Lab Progression

### Lab 01 – Network & Firewall Foundations
- pfSense deployment
- WAN/LAN segmentation
- Secure management access
- Baseline network validation

### Upcoming Labs
- Network discovery & service enumeration
- Vulnerability scanning & analysis
- Web application security testing
- Detection & logging validation
- Incident response workflows

---

## Documentation Approach

Each lab includes:
- Clear objectives
- Environment details
- Configuration steps
- Validation checks
- Security observations
- Evidence references

All sensitive data is sanitized prior to publication.

---

## Certifications Context

This lab reinforces hands-on skills aligned with:
- Defensive security analysis
- Adversarial testing fundamentals
- Network and application security assessment

The project emphasizes **practical application over exam simulation**.

---

## Status

**In Progress** — actively expanding lab scope and documentation.

---

## Disclaimer

This repository is for educational and professional development purposes only.  
All testing is performed in isolated lab environments under full authorization.
