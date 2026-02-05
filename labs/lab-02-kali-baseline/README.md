# Lab 02 — Kali Baseline (VMware)

## Goal
Establish a clean, repeatable Kali Linux baseline for the Enterprise-Style Information Security Lab.

This lab validates that the offensive testing platform is:
- Installed correctly
- Booting reliably
- Networked appropriately for isolated lab work
- Ready for future testing phases

## Environment
- Host OS: Windows 10/11
- Hypervisor: VMware Workstation 17 Player
- Guest OS: Kali Linux (pre-built VMware image)
- Architecture: amd64
- Network Mode: Host-only (isolated lab network)

## Validation Performed
- Successful VM boot to desktop
- Keyboard and mouse input captured correctly
- Network interface present and assigned IP
- Tooling available for security testing
- System identity confirmed

## Commands Captured
Outputs stored in `./outputs/`:

```bash
ip a
ip r
cat /etc/os-release
uname -a
whoami

## Evidence

Sanitized evidence stored in ./evidence/:

Desktop screenshot

Network configuration output

OS/version confirmation

## Notes

Any issues, fixes, or deviations from expected behavior are recorded in:
./notes/notes.md

## Outcome

Kali baseline validated and approved for use in subsequent security testing labs.

