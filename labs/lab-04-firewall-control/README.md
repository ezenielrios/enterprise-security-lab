# Lab 04 – Firewall Control & Traffic Enforcement

## Objective
Validate firewall behavior by observing how traffic is allowed or restricted across network boundaries using pfSense.

This lab focuses on understanding default firewall posture, interface trust boundaries, and how policy decisions affect traffic flow.

## Environment
- pfSense CE (Firewall)
- Kali Linux (Client)
- VMware Workstation
- Isolated lab network (192.168.59.0/24)

## Scope
- Review default pfSense firewall rules
- Validate LAN-to-WAN traffic behavior
- Confirm enforcement via client-side testing

## High-Level Actions
- Verified interface addressing and routing
- Observed baseline traffic allowance
- Prepared environment for rule-based enforcement testing

## Evidence
Supporting validation artifacts are stored in:
evidence/

-lab-04-default-lan-rules.png (baseline LAN rules before change)
-lab-04-icmp-block-rule.png (ICMP deny rule present/positioned
-lab-04-baseline-ping.png (ping allowed/working OR baseline)
-lab-04-kali-ping-blocked.png (ping blocked after rule)
-lab-04-firewall-logs.png (log entry showing block)

Screenshots and command outputs are sanitized and selectively included.

## Notes
Analytical observations and tool comparisons are documented in:
notes/


## Status
In progress — rule creation and enforcement testing to follow.
