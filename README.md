# Home Lab

A self-built cyber security lab where I build, attack and defend my own small network, then document every session. I'm a cyber security student; this repo is my hands-on record of learning, with a focus on SOC (Security Operations Centre) and defensive skills.

## Lab layout

```text
Windows 11 host (VirtualBox 7.2)
└── LabNet: NAT Network, 10.10.10.0/24
    └── lab-ubuntu-01   Ubuntu Server 26.04.1 LTS   (phase 1)
    └── Wazuh server    monitoring / SIEM           (phase 2, planned)
    └── Windows VM      "company" endpoint           (phase 3, planned)
    └── Kali Linux      attacker                     (phase 4, planned)
```

The lab network can reach the internet for updates but can't be reached from my home network. Before attack work in phase 4, the lab moves to a fully isolated Internal Network.

## Phases

| Phase | Goal | Status |
| --- | --- | --- |
| [1 – Foundation](phase-01-foundation/) | VirtualBox, isolated lab network, hardened Ubuntu Server, snapshot | ✅ Complete |
| 2 – Monitoring | Wazuh SIEM collecting logs and raising alerts | Planned | "Phase 2 – Monitoring: In progress"
| 3 – Windows | Windows endpoint joined to monitoring | Planned |
| 4 – Attack & detect | Attack the lab from Kali, investigate alerts, write incident reports | Planned |

## How write-ups are organised

Each phase has its own folder with a summary README and one write-up per session. Every write-up follows the same structure: Goal, Setup, Steps, Problems & fixes, What I learned, and Next steps.
