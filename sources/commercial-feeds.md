# 💼 Commercial Threat Intelligence Feeds

This document describes **commercial and private threat intelligence sources**, typically obtained via subscription or partnership.

---

## 🧩 1. Objectives

- Access **high-confidence, curated intelligence** not publicly available.  
- Gain insights on **advanced persistent threats (APTs)** and **targeted campaigns**.  
- Support **strategic and operational decision-making**.  

---

## 💡 2. Feed Types

| Feed Type | Description | Example Providers |
|------------|-------------|-------------------|
| **Tactical Feeds** | IOCs and indicators for SIEM/SOAR ingestion. | Recorded Future, Anomali, CrowdStrike Falcon X |
| **Operational Feeds** | Contextualized intelligence about campaigns and TTPs. | Mandiant, ThreatConnect, Kaspersky Threat Intelligence Portal |
| **Strategic Feeds** | Sector-focused and geopolitical reports. | FireEye, Intel 471, Flashpoint |
| **Industry ISAC Feeds** | Sector-specific sharing groups. | FS-ISAC, MS-ISAC, Health-ISAC |

---

## ⚙️ 3. Evaluation Criteria

When assessing a commercial feed (see also `enrichment/threat-feed-evaluation.md`):

- **Relevance** to your environment or sector  
- **Accuracy and timeliness** of published data  
- **Integration capabilities** (STIX/TAXII, API support)  
- **Data coverage**: malware, TTPs, vulnerabilities, phishing, etc.  
- **Cost, licensing, and redistribution rights**

---

## 🧠 4. Integration Examples

- Ingest feeds directly into **CTI platforms** (MISP, OpenCTI, ThreatConnect)  
- Use **SOAR playbooks** to automate IOC ingestion  
- Apply **confidence scoring** before forwarding to SIEM or detection systems  
- Combine with OSINT to **cross-validate indicators**  

---

## 🧰 5. Best Practices

- Mix **open-source and commercial** feeds for optimal coverage.  
- Establish **contracts and SLAs** defining update frequency and data quality.  
- Ensure **compliance** with internal and legal data handling policies.  
- Periodically **review ROI** and adjust subscriptions as needed.  
- Provide **feedback loops** with vendors to improve feed quality.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- Gartner – *Market Guide for Threat Intelligence Products and Services*  
- SANS – *Operationalizing Threat Intelligence*  
