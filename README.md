# Enterprise Security Lab

## Overview
This repository documents the design and execution of a hands-on, enterprise-style information security lab built using entirely free and open-source tools. The lab is structured to simulate real-world security operations, including network discovery, vulnerability assessment, adversarial testing, and defensive validation.

The goal of this project is to demonstrate practical security engineering skills through repeatable workflows, clear documentation, and evidence-based analysis rather than tool screenshots alone.

---

## Objectives
- Design a realistic multi-segment lab environment
- Perform structured security testing aligned with enterprise practices
- Document findings with professional clarity and restraint
- Emphasize methodology, scope control, and ethical testing
- Bridge offensive and defensive security perspectives

---

## Lab Architecture (High-Level)
- Virtualized environment using VMware
- pfSense firewall for routing, segmentation, and traffic control
- Isolated LAN and WAN simulation
- Attacker, target, and management segments
- Logging and inspection points for defensive visibility

> Detailed diagrams and configuration notes are maintained in the `/docs` directory.

---

## Tools & Technologies
- pfSense (Firewall & Network Segmentation)
- Kali Linux (Security Testing Platform)
- Nmap (Network Discovery & Enumeration)
- OpenVAS / Greenbone (Vulnerability Assessment)
- Burp Suite Community (Web Application Testing)
- Docker (Vulnerable Application Hosting)
- Linux & Windows test systems

Only tools appropriate to each lab phase are used to avoid unnecessary noise.

---

## Repository Structure

enterprise-security-lab/
├── docs/ # Architecture notes, diagrams, and methodology
├── labs/ # Individual lab exercises and walkthroughs
├── evidence/ # Sanitized outputs, logs, and findings
├── README.md # Project overview (this file)
└── LICENSE


---

## Methodology
Each lab follows a consistent structure:
1. **Objective & Scope Definition**
2. **Environment Preparation**
3. **Execution & Observation**
4. **Findings & Analysis**
5. **Defensive Implications**
6. **Lessons Learned**

This ensures results are repeatable, explainable, and defensible.

---

## Ethical Use & Scope
All testing documented in this repository is performed in isolated, intentionally vulnerable lab environments. No testing is conducted against systems without explicit authorization.

---

## Status
**In Progress**  
Labs are added incrementally to ensure accuracy, clarity, and relevance.

---

## Author
**Ezeniel Rios**  
Cybersecurity Practitioner | Security Analysis & Testing  

