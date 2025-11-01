# 🌍 Open-Source Intelligence (OSINT) Sources

This document lists and categorizes **public and open-source threat intelligence sources** that analysts can use for investigation, enrichment, and situational awareness.

---

## 🧩 1. Objectives

- Collect and analyze threat data from **trusted public sources**.  
- Support **incident response, detection engineering, and enrichment**.  
- Build **contextual awareness** around campaigns, TTPs, and threat actors.

---

## 🌐 2. OSINT Platforms

| Platform | Type | Description |
|-----------|------|-------------|
| **MISP** | Community | Open-source threat intelligence platform for sharing IOCs and events. |
| **OpenCTI** | Platform | Structured threat intelligence management system with ATT&CK mapping. |
| **AlienVault OTX** | Feed | Collaborative threat feed sharing community. |
| **Abuse.ch** | Feed | Repositories of malicious URLs, botnets, and malware indicators. |
| **Malpedia** | Repository | Open collection of malware families and analysis. |
| **URLhaus** | Feed | Database of malicious URLs submitted by researchers. |
| **ThreatFox** | Feed | Repository of verified IoCs shared by the community. |
| **Any.Run / Hybrid Analysis** | Sandbox | Online malware analysis and behavioral data. |

---

## 🔎 3. Intelligence Communities & Projects

| Community | Region | Focus |
|------------|---------|-------|
| **TheHive Project** | Global | Incident response and case management platform. |
| **CIRCL Luxembourg** | Europe | MISP community and OSINT sharing initiatives. |
| **Shadowserver Foundation** | Global | Botnet and vulnerability monitoring reports. |
| **AbuseIPDB** | Global | Collaborative database for malicious IPs. |
| **Spamhaus / PhishTank** | Global | Phishing and spam domain tracking. |

---

## 🧠 4. Use Cases

- IOC enrichment (hashes, IPs, domains)  
- TTP validation and ATT&CK mapping  
- Correlate threat actor campaigns  
- Early warning of sector-specific activity  
- Support for threat hunting and detection engineering  

---

## ⚙️ 5. Best Practices

- Verify data reliability and **confidence** levels before ingestion.  
- Automate retrieval via **API** where possible (OTX, Abuse.ch, etc.).  
- Maintain a **whitelist** to reduce false positives.  
- Integrate OSINT data into a **MISP** or **OpenCTI** instance.  
- Always **cite and timestamp** OSINT sources.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- ENISA – *Open Source Threat Intelligence Practices*  
- MISP Project – *OSINT Feeds Documentation*  
