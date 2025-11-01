# 🧩 IOC Enrichment Guide

**IOC Enrichment** adds context to Indicators of Compromise (IoCs) to improve **detection, threat hunting, and intelligence analysis**.

---

## 🧭 1. Objectives

- Validate and verify IoCs from internal or external sources.  
- Add context: associated TTPs, threat actors, campaigns.  
- Determine relevance and priority for your environment.  
- Facilitate automated ingestion into SIEM, EDR, or CTI platforms.

---

## ⚙️ 2. Enrichment Workflow

1. **Validation**
   - Check IOC syntax, hash integrity, domain registration, and IP reputation.
   - Discard outdated or false-positive indicators.

2. **Contextualization**
   - Associate IoCs with:
     - MITRE ATT&CK techniques
     - Diamond Model components
     - Known threat actors or campaigns

3. **Cross-Reference Sources**
   - Compare IOC against:
     - Internal telemetry and incident logs
     - Threat intelligence feeds
     - Open-source intelligence (OSINT)
     - Malware analysis reports

4. **Tag & Score**
   - Assign metadata: confidence level, impact, environment relevance, and expiration date.

5. **Format for Automation**
   - Convert into structured formats like STIX, JSON, CSV, or platform-specific ingestion formats.

---

## 🧠 3. Example Enrichment Table

| IOC | Type | Source | Associated TTP | Campaign | Threat Actor | Confidence |
|-----|------|--------|----------------|----------|--------------|------------|
| 1a2b3c… | File hash | MISP feed | T1059.001 – PowerShell | Ransomware-Financial-Q4 | FIN7 | High |
| bad-domain.com | Domain | OSINT | T1071 – Web Protocol | Phishing-Executive-2025 | APT29 | Medium |
| 192.168.1.100 | IP | Internal logs | T1071.004 – Custom C2 | Unknown | Unknown | Low |

---

## 🧰 4. Tools & Techniques

| Task | Tools / Methods |
|------|----------------|
| Malware analysis | Cuckoo Sandbox, Hybrid Analysis |
| Domain/IP investigation | Passive DNS, WHOIS, ThreatCrowd, AbuseIPDB |
| IOC correlation | MISP, OpenCTI, internal CTI platform |
| TTP mapping | MITRE ATT&CK Navigator, custom scripts |

---

## 🔄 5. Best Practices

- **Automate enrichment** where possible but validate manually for critical indicators.  
- Maintain **source attribution and confidence**.  
- Integrate enrichment with **SOC, IR, and threat hunting workflows**.  
- Track **changes over time** (e.g., domain IP shifts, malware hash changes).  
- Ensure **structured storage** for reuse in detection and reporting.

---

## 📚 References

- MISP Project – *Indicators Management & Correlation*  
- MITRE ATT&CK – *TTP Mapping*  
- SANS – *Practical Threat Intelligence for SOC Teams*  
- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*
