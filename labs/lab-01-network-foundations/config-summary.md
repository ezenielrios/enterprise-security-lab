# Configuration Summary – Lab 01

## Firewall
- Platform: pfSense CE 2.7.2
- Deployment: VMware Workstation
- Disk: Default pfSense installer configuration (no custom partitioning)

## Interfaces
- WAN (em0)
  - Type: NAT (VMnet8)
  - Addressing: DHCP
- LAN (em1)
  - Type: Host-only (VMnet1)
  - Address: 192.168.59.1/24

## Services
- DHCP enabled on LAN
  - Range: 192.168.59.100–199
- WebConfigurator enabled (HTTPS)
- Default firewall rules in place for LAN management access

## Notes
This configuration establishes a stable perimeter baseline for subsequent testing and monitoring labs.

