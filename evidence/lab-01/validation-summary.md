# Lab 01 – Validation Summary

This document summarizes the validation steps performed to confirm the pfSense firewall and network foundation are functioning as intended.

## Management Access
- pfSense WebConfigurator reachable over HTTPS
- Access confirmed at:
https://192.168.59.1
- Self-signed certificate warning acknowledged as expected

## Interface Verification
- WAN interface assigned to NAT network (VMnet8)
- LAN interface assigned to Host-only network (VMnet1)
- LAN IP address confirmed as `192.168.59.1/24`

## Service Status
- WebConfigurator (nginx) confirmed listening on TCP port 443
- DHCP service active on LAN interface
- Host system received valid LAN IP address

## Conclusion
The firewall perimeter and network segmentation are operational and ready to support subsequent discovery and security testing labs.
