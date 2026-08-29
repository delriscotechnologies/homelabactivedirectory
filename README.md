<h1 align="center">ACTIVE DIRECTORY HOME LAB</h1>

<p align="center">
  A Splunk-powered Active Directory homelab for learning identity administration, Windows telemetry, controlled attack simulation, and detection engineering.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabactivedirectory/">Full Write-Up</a>
</p>

---

Active Directory Home Lab documents an isolated four-machine detection environment. The project combines Active Directory auditing, Sysmon telemetry, Splunk Universal Forwarder, Splunk searches, and an authorized Hydra simulation.

## Lab design

The addresses below are historical, private lab values. They are not production endpoints.

| System | Lab address | Purpose |
| --- | --- | --- |
| Windows Server | `192.168.64.7` | Active Directory Domain Services and DNS |
| Ubuntu Server | `192.168.64.10` | Splunk indexer and web interface |
| Windows 10 Pro 22H2 | `192.168.64.100` | Domain endpoint, Sysmon, and Splunk forwarder |
| Kali Linux | `192.168.64.250` | Authorized authentication testing |

Windows 10 Pro 22H2 is retained only as a historical, isolated training endpoint. Standard support ended on October 14, 2025. Use a supported Windows release for any new connected lab unless the legacy system is covered by Extended Security Updates.

## Lab-only identities

| Identity | Purpose | Handling |
| --- | --- | --- |
| `CFDR` | Disposable domain account used in the controlled RDP test | Historical lab value; never reuse or retain its password |
| Lab administrator | Domain setup and policy administration | Create a unique credential and destroy it with the lab |

Screenshots may show lab-only hostnames, private addresses, identifiers, or disposable credentials. None were used or reused on personal, production, or external systems.

## Reproduce safely

1. Place every VM on an isolated virtual network. Do not bridge the lab to a production LAN or expose its services to the internet.
2. Point domain members to the domain controller for DNS. Configure external resolvers only as forwarders on the domain controller.
3. Allow Splunk ingestion on port `9997` only from the authorized forwarder addresses and validate TLS certificates.
4. Permit RDP from the Kali host to the test endpoint only for the controlled exercise, then remove the rule.
5. Use disposable accounts and wordlists that have never been used outside the lab.
6. At teardown, export only sanitized evidence, revoke lab credentials, remove attack files, and delete the VMs and snapshots.

> Build and operate this lab only on systems and networks you own or are explicitly authorized to test. Never publish personal or production secrets.

## Repository contents

This repository contains the write-up, security guidance, and selected screenshots. It does not contain VM provisioning automation, certificates, production credentials, or production-ready infrastructure.

## References

- [Active Directory Domain Services](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [Sysmon documentation](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Splunk documentation](https://docs.splunk.com/)
- [Sysmon Modular](https://github.com/olafhartong/sysmon-modular)
- [Kali Linux Hydra documentation](https://www.kali.org/tools/hydra/)
- [Ubuntu Server documentation](https://ubuntu.com/server/docs)
- [Windows 10 lifecycle notice](https://learn.microsoft.com/en-us/lifecycle/announcements/windows-10-22h2-end-of-support-update)
