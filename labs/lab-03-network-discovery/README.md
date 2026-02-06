# Lab 03 – Network Discovery & Host Enumeration

## Overview
This lab focuses on identifying active hosts within the local network segment using passive and active discovery techniques. The objective is to establish a reliable baseline of reachable systems prior to deeper service enumeration or vulnerability assessment.

All discovery activities were performed from a controlled Kali Linux environment within an isolated lab network.

---

## Objectives
- Confirm network configuration and assigned IP addressing
- Identify active hosts on the local subnet
- Validate results using multiple discovery techniques
- Document findings using sanitized evidence suitable for professional reporting

---

## Environment
- **Attacking Host:** Kali Linux (VMware)
- **Network Type:** NAT / Isolated Lab Network
- **Subnet Observed:** 192.168.133.0/24
- **Tools Used:**
  - `ip`
  - `arp-scan`
  - `nmap`

---

## Methodology

### 1. Interface & IP Confirmation
The active network interface and assigned IP address were verified to ensure correct network placement prior to scanning.

Command used:
ip a

This confirmed:

Active interface (eth0)

Assigned IPv4 address within the expected subnet

### 2. ARP-Based Host Discovery

An ARP scan was conducted to identify live hosts responding at Layer 2. This method is effective for discovering hosts that may not respond to higher-layer probes.

Command used:
sudo arp-scan --localnet

Results identified multiple active hosts on the local network, including the default gateway and additional virtual systems.

### 3. Active Host Discovery (ICMP)

To validate ARP results and identify additional responding systems, an ICMP-based discovery scan was executed using Nmap.

Command used:sudo nmap -sn 192.168.133.0/24

This scan confirmed:

Multiple active hosts

Low-latency responses consistent with a local virtualized network

MAC address attribution indicating VMware-managed interfaces

## Findings Summary

The local subnet contains multiple reachable hosts.

Discovery results were consistent across ARP and ICMP-based methods.

No unexpected or external hosts were identified.

Network visibility is sufficient to proceed to service-level enumeration.

## Evidence

Sanitized supporting artifacts are available in:
evidence/screenshots/

Included artifacts:

Interface and IP confirmation output

ARP scan results

Nmap host discovery output

All evidence has been reviewed to remove sensitive or identifying information while preserving technical validity.

## Key Takeaways

Multiple discovery techniques should be used to ensure accuracy.

ARP-based discovery provides strong visibility in local networks.

Establishing a reliable host baseline is critical before deeper testing phases.

## Next Steps

Lab 04: Service Enumeration & Port Scanning

Identify exposed services on discovered hosts

Begin protocol- and service-specific analysis
