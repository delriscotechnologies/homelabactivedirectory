<h1 align="center">ACTIVE DIRECTORY HOME LAB</h1>

<p align="center">
  A Splunk-powered Active Directory homelab for learning identity administration, Windows telemetry, controlled attack simulation, and detection engineering.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabactivedirectory/">Full Write-Up</a>
</p>

---

Active Directory Home Lab documents an isolated four-machine detection environment using Active Directory, Sysmon, Splunk Universal Forwarder, Splunk searches, and a controlled Hydra simulation.

The lab focuses on collecting Windows and Active Directory telemetry and using it to investigate authentication and endpoint activity.

> Build and operate this lab only on systems and networks you own or are explicitly authorized to test. Never publish real credentials, production data, or sensitive evidence.

## References

- [Active Directory Domain Services](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
- [Sysmon documentation](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)
- [Splunk documentation](https://docs.splunk.com/)
- [Sysmon Modular](https://github.com/olafhartong/sysmon-modular)
- [Kali Linux Hydra documentation](https://www.kali.org/tools/hydra/)
