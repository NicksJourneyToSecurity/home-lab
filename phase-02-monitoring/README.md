# Phase 2 – Monitoring

**Status:** In progress (Wazuh server built; agent and test alerts next)

## What's been built so far

- git set up on my PC so this repo is committed from the command line as NicksJourneyToSecurity
- `lab-wazuh-01`: Ubuntu Server 24.04.5 LTS on a static IP (`10.10.10.10`), disk extended to use the full 50GB
- Wazuh 4.14.10 all-in-one: manager, indexer and dashboard running
- UFW firewall: incoming denied by default; SSH, dashboard and agent registration allowed
- Dashboard reachable from my PC only, via a LabNet port forward on `127.0.0.1:8443`
- Snapshots: `01-clean-base`, `02-wazuh-installed`

## Still to do

- Allow agent log traffic (1514/tcp) in the firewall
- Connect `lab-ubuntu-01` as a Wazuh agent
- Trigger and investigate test alerts

## Sessions

| Session | Summary |
| --- | --- |
| [Session 02](2026-11-09-session-02.md) | Git setup, Wazuh server build and dashboard access |
