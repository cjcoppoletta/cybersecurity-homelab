# Cybersecurity Home Lab

A self-hosted blue team security lab built from open source tools to practice 
SOC analysis as well as incident response.

## Lab Environment

| Tool | Category | Purpose |
|------|----------|---------|
| Wazuh | SIEM/XDR | Log ingestion, alerting, endpoint monitoring | Case Management | Incident tracking and response |
| MISP | Threat Intelligence | IOC sharing and enrichment |
| Kali Linux | Attack Simulation | Offensive tooling for detection testing |
| Metasploitable 2 | Vulnerable Target | Attack target for lab scenarios |
| Windows Server 2022 | Endpoint/IAM | Active Directory and Windows log monitoring |

## Network Architecture

- Hypervisor: VirtualBox on Windows Host
- Lab Network: NAT Network (LabNet) + Host-Only Adapter (192.168.56.x)
- All VMs communicate over LabNet
- Host-Only adapter enables browser access to dashboards from Windows host

## Skills

- SIEM deployment and agent enrollment (Linux and Windows endpoints)
- Network segmentation and VM networking configuration
- Endpoint log collection and centralized monitoring
- Incident case management workflow
- Threat intelligence platform integration

## Lab Sections

- [Wazuh SIEM](./wazuh/README.md)
- [Windows Server 2022](./windows-server/README.md)
- [TheHive + MISP](./thehive-misp/README.md)
