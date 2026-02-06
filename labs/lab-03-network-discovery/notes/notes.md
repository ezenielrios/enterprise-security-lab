# Lab 03 – Notes: arp-scan vs nmap Host Discovery

## Purpose of This Lab
This lab focuses on validating active hosts on a local network segment and understanding how different discovery tools operate at different layers of the network stack.

The goal is not just to enumerate hosts, but to demonstrate correct tool selection, sequencing, and interpretation of results.

---

## Tool Comparison

### arp-scan
**Layer:** OSI Layer 2 (Data Link)

**How it works:**
- Sends ARP requests directly on the local broadcast domain
- Does not rely on IP routing or ICMP responses
- Identifies hosts that respond to ARP, even if higher-layer traffic is filtered

**Strengths:**
- Very fast and reliable on local networks
- Discovers hosts that block ICMP (ping)
- Effective for identifying virtual infrastructure and hidden hosts

**Limitations:**
- Only works on the local subnet
- Cannot scan routed networks
- Limited service visibility (host presence only)

---

### nmap (-sn)
**Layer:** OSI Layer 3/4 (Network / Transport)

**How it works:**
- Uses ICMP echo requests, TCP SYN probes, and ARP (when applicable)
- Determines host availability without scanning ports

**Strengths:**
- Flexible across local and routed networks
- Integrates cleanly into larger reconnaissance workflows
- Provides MAC vendor information when available

**Limitations:**
- ICMP or probe traffic may be filtered
- May miss hosts that only respond at Layer 2

---

## Why Both Tools Were Used
Using both arp-scan and nmap provides layered validation:

1. **arp-scan** confirms which hosts physically exist on the local network
2. **nmap -sn** validates host reachability using IP-based methods
3. Differences between results may indicate filtering, segmentation, or host-based controls

This mirrors real-world reconnaissance workflows used during internal security assessments.

---

## Analyst Takeaway
Effective network discovery is not about running a single tool. It requires:
- Understanding protocol behavior
- Selecting tools appropriate to network scope
- Interpreting discrepancies as signals, not errors

This lab establishes a reliable baseline for deeper enumeration in future phases.
