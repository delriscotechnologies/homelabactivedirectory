<h1 align="center">ACTIVE DIRECTORY HOME LAB</h1>

<p align="center">
  A Splunk-powered Active Directory homelab for learning identity administration, Windows telemetry, controlled attack simulation, and detection engineering.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabactivedirectory/">Full Write-Up</a>
</p>

---

Active Directory Home Lab documents an isolated four-machine detection environment. Windows Server provides Active Directory Domain Services and DNS, a domain-joined Windows 10 endpoint generates security telemetry, Ubuntu hosts Splunk, and Kali Linux produces controlled authentication activity for analysis. Windows 10 Pro 22H2 appears here only as a historical, isolated training endpoint; its standard support ended on October 14, 2025, so it should not be used for a connected or production deployment without Extended Security Updates.

The lab combines Active Directory auditing, Sysmon endpoint telemetry, Splunk Universal Forwarder, Splunk search and correlation, and authorized Hydra simulations. This repository contains the project write-up, security guidance, and selected screenshots captured inside the isolated lab. Those screenshots may show lab-only hostnames, private addresses, user names, identifiers, and disposable credentials created specifically for the exercise. They were used only in this sandbox and were never used or reused on personal, production, or external systems. The repository does not contain VM provisioning automation, certificates, production credentials, or production-ready infrastructure.

> Build and operate this lab only on systems and networks you own or are explicitly authorized to test. Treat every visible account and password as historical lab evidence, never reuse lab credentials elsewhere, and never publish personal or production secrets.

## References

- [Microsoft Active Directory Domain Services documentation](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [Microsoft Sysmon documentation](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Splunk documentation](https://docs.splunk.com/)
- [Sysmon Modular repository](https://github.com/olafhartong/sysmon-modular)
- [Kali Linux Hydra documentation](https://www.kali.org/tools/hydra/)
- [Ubuntu Server documentation](https://ubuntu.com/server/docs)
- [Windows 10 lifecycle notice](https://learn.microsoft.com/en-us/lifecycle/announcements/windows-10-22h2-end-of-support-update)
