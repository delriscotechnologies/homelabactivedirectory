<h1 align="center">ACTIVE DIRECTORY HOME LAB</h1>

<p align="center">
  A Splunk-powered Active Directory homelab for learning identity administration, Windows telemetry, controlled attack simulation, and detection engineering.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabactivedirectory/">Full Write-Up</a>
</p>

---

Active Directory Home Lab documents an isolated four-machine detection environment. Windows Server provides Active Directory Domain Services and DNS, a domain-joined Windows 10 endpoint generates security telemetry, Ubuntu hosts Splunk, and Kali Linux produces controlled authentication activity for analysis.

The lab combines Active Directory auditing, Sysmon endpoint telemetry, Splunk Universal Forwarder, Splunk search and correlation, and authorized Hydra simulations. This repository contains the project write-up and security guidance; it does not contain VM provisioning automation, credentials, certificates, captured evidence, or production-ready infrastructure.

> Build and operate this lab only on systems and networks you own or are explicitly authorized to test. Windows and Splunk telemetry can contain credentials, private addresses, host details, user names, alerts, and other sensitive evidence; never commit real lab data to a public repository.

## References

- [Microsoft Active Directory Domain Services documentation](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [Microsoft Sysmon documentation](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Splunk documentation](https://docs.splunk.com/)
- [Sysmon Modular repository](https://github.com/olafhartong/sysmon-modular)
- [Kali Linux Hydra documentation](https://www.kali.org/tools/hydra/)
- [Ubuntu Server documentation](https://ubuntu.com/server/docs)
