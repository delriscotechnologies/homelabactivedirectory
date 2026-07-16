<h1 align="center">ACTIVE DIRECTORY HOME LAB</h1>

<p align="center">
  A four-VM detection lab for identity, endpoint telemetry, controlled attack simulation, and Splunk analysis.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabsoc/"><strong>Full Write-Up</strong></a>
</p>

---

This repository documents an isolated Active Directory environment built to make authentication, endpoint activity, attack simulation, and defensive analysis visible in one place.

The lab connects a Windows Server domain controller, a domain-joined Windows 10 endpoint, an Ubuntu Splunk server, and a Kali Linux attacker VM. Windows Event Logs and Sysmon telemetry flow into Splunk, where controlled activity can be searched and correlated without touching a production network.

> Use this lab only on systems and networks you own or have explicit permission to test. Every address, account, hostname, and credential shown here belongs to an isolated training sandbox.
