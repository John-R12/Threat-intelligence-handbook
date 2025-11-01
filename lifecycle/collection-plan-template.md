# 📋 Threat Intelligence Collection Plan Template

A **Collection Plan** defines *what information* needs to be collected, *why*, *from where*, and *how often*.  
It ensures that data collection is aligned with intelligence requirements and operational priorities.

---

## 🧭 Purpose

- Translate **Priority Intelligence Requirements (PIRs)** into actionable data collection tasks.  
- Define **sources**, **methods**, and **responsibilities** for gathering relevant intelligence.  
- Enable **traceability** between intelligence needs and collected data.  
- Avoid redundant or low-value data collection.

---

## 🧩 1. Intelligence Requirements

| ID | Requirement Type | Description | Priority | Stakeholder |
|----|------------------|-------------|-----------|--------------|
| PIR-01 | Strategic | Identify top 3 threat actors targeting the financial sector. | High | CISO |
| PIR-02 | Operational | Monitor exploitation of new critical vulnerabilities (CVSS ≥ 9). | High | SOC Lead |
| PIR-03 | Tactical | Track new phishing domains impersonating our brand. | Medium | Threat Hunter |

> **Tip:** Keep your list of PIRs short (5–10 max). Focus on decisions that intelligence will enable.

---

## 🌐 2. Data Sources

| Source Name | Type | Access Method | Frequency | Confidence | Notes |
|--------------|------|---------------|------------|-------------|-------|
| MISP Community Feed | Open Source | TAXII API | Daily | High | Automated ingestion |
| ThreatConnect Premium | Commercial | API | Hourly | High | Integrated with SIEM |
| VirusTotal Intelligence | Paid | Web/API | On-demand | Medium | File and domain enrichment |
| Internal SOC Alerts | Internal | Syslog | Continuous | High | Primary detection telemetry |
| Dark Web Monitoring | External | Vendor Feed | Weekly | Medium | Requires sanitization |

> Include **source diversity** (OSINT, commercial, community, internal).  
> Rate each source for reliability and confidence.

---

## ⚙️ 3. Collection Methods

| Method | Description | Tools / Scripts | Responsible Team |
|---------|--------------|------------------|------------------|
| Automated Feed Pull | Scheduled ingestion from APIs | TAXII client, MISP Sync | CTI Analyst |
| Manual Collection | Analyst-driven collection and validation | Browser, scraper, RSS | CTI Team |
| Integration with SIEM | Automated IOC ingestion for detection | Splunk / Sentinel | Detection Engineering |
| Incident Report Review | Extract intelligence from IR cases | Internal templates | SOC / IR Team |

---

## 🧠 4. Data Management

| Policy | Description |
|---------|-------------|
| **Storage** | All collected data must be stored in the central CTI platform or repository. |
| **Retention** | Maintain data for 12–24 months depending on classification. |
| **Classification** | Tag data with TLP and confidence level (Low / Medium / High). |
| **Quality Control** | Review new sources quarterly for accuracy and redundancy. |

---

## 🕓 5. Review & Maintenance

- Review collection plan **every quarter** or when new intelligence requirements emerge.  
- Track **source performance** (usefulness, accuracy, false positives).  
- Update the plan based on **feedback from analysts and stakeholders**.  
- Document **retired sources** and **new integrations**.

---

## 🧩 Example — Collection Alignment Matrix

| PIR | Collection Source | Method | Expected Output | Status |
|------|-------------------|---------|------------------|--------|
| PIR-01 | MISP, ThreatConnect | API Feeds | Actor names, TTPs | Active |
| PIR-02 | CVE Feeds, Vendor Advisories | Automated | CVE reports | Active |
| PIR-03 | DomainTools, PhishTank | Manual/API | Suspicious domains | Active |

---

## 🧰 Best Practices

- Keep collection **focused and justified** by PIRs.  
- Avoid “collect everything” — aim for *quality over quantity*.  
- Use **confidence scoring** and **source reliability tracking**.  
- Automate where possible, but validate manually where needed.  
- Maintain **documentation for reproducibility**.

---

## 📚 References
- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- SANS – *Building a Threat Intelligence Program*  
- MITRE – *Cyber Threat Intelligence and Collection Management*  
- ENISA – *Threat Intelligence Platform Guidance*
