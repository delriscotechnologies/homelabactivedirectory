<h1 align="center">AI SOC HOMELAB</h1>

<p align="center">
  An AI-assisted security homelab with Wazuh, Hermes Agent and MCP for endpoint monitoring, investigation and incident tracking.
</p>

<p align="center">
  <a href="https://delriscotechnologies.github.io/homelabactivedirectory/aisochomelab/">Full Write-Up</a>
</p>

---

AI SOC Homelab documents a two-VM environment: Windows 11 runs the Wazuh agent, while Ubuntu hosts Wazuh Manager, Indexer, Dashboard, Hermes Agent, Ollama and a Docker-based MCP server.

The write-up covers file integrity monitoring, VirusTotal enrichment, rule-based Active Response, vulnerability detection and CIS configuration assessment. Hermes accesses Wazuh through MCP, Discord provides a conversational interface, and Sentinel forwards selected alerts to Notion.

## References

- [Wazuh documentation](https://documentation.wazuh.com/current/)
- [Model Context Protocol](https://modelcontextprotocol.io/)
- [Ollama documentation](https://docs.ollama.com/)
- [VirusTotal documentation](https://docs.virustotal.com/)
