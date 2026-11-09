# Phase 1 – Foundation

**Status:** ✅ Complete (2026-11-09)

## What was built

- Oracle VirtualBox 7.2 on a Windows 11 host, with VMs stored on a separate HDD
- `LabNet`: a NAT Network (`10.10.10.0/24`) keeping lab VMs off my home network
- `lab-ubuntu-01`: Ubuntu Server 26.04.1 LTS, installed from a checksum-verified ISO
- Basic hardening: full updates, correct timezone, UFW firewall allowing only SSH, listening services checked, automatic security updates confirmed
- Snapshot `01-clean-hardened` as a restore point

## Sessions

| Session | Summary |
| --- | --- |
| [Session 01](2026-11-09-session-01.md) | Full phase 1 build, from VirtualBox install to snapshot |
