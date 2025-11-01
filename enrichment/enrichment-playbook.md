# 🧰 Enrichment Playbook

This playbook provides **practical guidance for enriching IoCs, TTPs, and incidents** with context, relevance, and actionable intelligence.  
It integrates best practices, tools, and structured workflows for CTI teams.

---

## 🧩 1. Objectives

- Transform raw indicators into **actionable intelligence**.  
- Add **context, confidence, and relevance**.  
- Support **threat hunting, detection, and incident response**.  
- Ensure **consistent, traceable enrichment workflows**.

---

## ⚙️ 2. Enrichment Workflow

1. **Validate Indicators**  
   - Confirm format, integrity, and authenticity of IoCs.  
   - Remove duplicates or outdated entries.

2. **Contextualize**  
   - Map IoCs to:
     - MITRE ATT&CK techniques  
     - Diamond Model components (Adversary, Capability, Infrastructure, Victim)  
     - Known campaigns or threat actors  

3. **Cross-Reference External Sources**  
   - Open-source intelligence (OSINT)  
   - Threat feeds (internal and external)  
   - Malware analysis reports  
   - Security research publications  

4. **Add Metadata & Scoring**  
   - Confidence (High / Medium / Low)  
   - Relevance (Environment-specific)  
   - Impact potential  
   - Source attribution  
   - Expiration or review date  

5. **Format for Consumption**  
   - STIX/TAXII for automation  
   - JSON, CSV, or platform-specific ingestion formats  
   - Include human-readable summaries for analysts and SOC teams  

6. **Correlate & Integrate**  
   - Link enriched IoCs to campaigns, TTPs, and incidents  
   - Feed findings into SIEM, SOAR, CTI platforms  

7. **Document & Review**  
   - Maintain logs of enrichment actions  
   - Update based on feedback from SOC, IR, and CTI analysts

---

## 🧠 3. Example Enrichment Table

| IOC | Type | Source | Associated TTP | Campaign | Threat Actor | Confidence | Relevance |
|-----|------|--------|----------------|----------|--------------|------------|-----------|
| 1a2b3c… | File hash | MISP feed | T1059.001 – PowerShell | Ransomware-Financial-Q4 | FIN7 | High | High |
| bad-domain.com | Domain | OSINT | T1071 – Web Protocol | Phishing-Executive-2025 | APT29 | Medium | High |
| 192.168.1.100 | IP | Internal logs | T1071.004 – Custom C2 | Unknown | Unknown | Low | Medium |

---

## 🧰 4. Tools & Techniques

| Task | Tools / Methods |
|------|----------------|
| Malware analysis | Cuckoo Sandbox, Hybrid Analysis |
| Domain/IP investigation | Passive DNS, WHOIS, ThreatCrowd, AbuseIPDB |
| IOC correlation | MISP, OpenCTI, internal CTI platform |
| TTP mapping | MITRE ATT&CK Navigator, custom scripts |
| Automation | Python scripts, SOAR playbooks, STIX/TAXII pipelines |

---

## 🔄 5. Best Practices

- **Automate repetitive enrichment tasks** but validate critical indicators manually.  
- Maintain **source attribution and confidence metadata** for traceability.  
- Integrate enriched data into **SOC dashboards, hunting workflows, and detection engineering**.  
- Use **consistent naming conventions** for campaigns, TTPs, and threat actors.  
- Periodically **review and prune outdated or low-confidence indicators**.  
- Encourage **feedback loops** from SOC, IR, and CTI teams for continuous improvement.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- MISP Project – *Indicators Management & Correlation*  
- MITRE ATT&CK – *TTP Mapping*  
- SANS – *Practical Threat Intelligence for SOC Teams*
