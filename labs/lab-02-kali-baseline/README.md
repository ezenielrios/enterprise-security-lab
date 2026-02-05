# Lab 02 – Kali Linux Baseline Network Configuration

## Overview
This lab establishes and validates the baseline network configuration of a Kali Linux virtual machine within the enterprise-style security lab environment. A verified baseline ensures that subsequent security testing activities are conducted from a known, controlled state and that observed results are attributable to testing actions rather than environmental inconsistencies.

## Objectives
- Confirm successful deployment and operation of Kali Linux
- Validate active network interfaces and IP assignment
- Establish a documented baseline for future comparison
- Ensure the testing host is network-ready before reconnaissance and assessment activities

## Environment
- **Operating System:** Kali Linux (Rolling)
- **Virtualization Platform:** VMware Workstation
- **Network Mode:** Host-only / Lab-isolated network
- **Role:** Security testing workstation

## Methodology
The following steps were performed to validate the baseline configuration:

1. Logged into the Kali Linux desktop environment
2. Opened a terminal session
3. Executed the `ip a` command to enumerate:
   - Available network interfaces
   - Interface state (UP/DOWN)
   - Assigned IPv4 address
4. Reviewed output to confirm:
   - Primary interface is active
   - IP address is assigned via the expected network segment
   - No unexpected interfaces or configurations are present

## Results
- The primary network interface (`eth0`) is operational and in an **UP** state
- An IPv4 address was successfully assigned
- Network configuration aligns with the intended isolated lab design
- Kali is ready to proceed with reconnaissance and security testing tasks

## Evidence
Sanitized evidence supporting this validation is located in:
evidence/screenshots/


Artifacts include:
- Terminal output confirming interface status and IP assignment

No sensitive credentials or external network identifiers are exposed.

## Security Considerations
- Network isolation limits unintended exposure to production systems
- Only baseline validation commands were executed
- No active scanning or exploitation occurred during this lab

## Lessons Learned
- Verifying baseline configuration prevents misattribution of findings later in the lab sequence
- Minimal, targeted evidence improves clarity and professionalism
- Consistent documentation simplifies future troubleshooting and comparisons

## Next Steps
- Proceed to **Lab 03: Network Discovery and Service Enumeration**
- Begin controlled reconnaissance using Nmap against designated lab targets

---

**Lab Status:** Complete  
**Prepared by:** Ezeniel Rios



