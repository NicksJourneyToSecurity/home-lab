# Phase 2 – Monitoring

**Status:** In progress (agent connected; test alerts next)

## What's been built so far

- git set up on my PC so this repo is committed from the command line as NicksJourneyToSecurity
- `lab-wazuh-01`: Ubuntu Server 24.04.5 LTS on a static IP (`10.10.10.10`), disk extended to use the full 50GB
- Wazuh 4.14.10 all-in-one: manager, indexer and dashboard running
- UFW firewall: incoming denied by default; SSH (22), dashboard (443), agent logs (1514) and agent registration (1515) allowed
- LabNet port forwards on `127.0.0.1` only: dashboard (8443) and SSH to both VMs (2222, 2223)
- `lab-ubuntu-01` connected as Wazuh agent `001`, status active
- Snapshots: `01-clean-base`, `02-wazuh-installed`

## Still to do

- Trigger and investigate test alerts

## Sessions

| Session | Summary |
| --- | --- |
| [Session 02](2026-11-09-session-02.md) | Git setup, Wazuh server build and dashboard access |
| [Session 03](2026-11-10-session-03.md) | Firewall fix, SSH access and first agent connected |
