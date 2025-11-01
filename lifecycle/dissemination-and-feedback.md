# 📢 Dissemination & Feedback

The value of Cyber Threat Intelligence (CTI) depends on **how effectively it is shared and used**.  
Intelligence must reach the right audience, in the right format, at the right time — and evolve based on their feedback.  
This phase ensures that CTI is **actionable, trusted, and continuously improved**.

---

## 🧩 1. Dissemination Principles

| Principle | Description |
|------------|--------------|
| **Timeliness** | Deliver intelligence early enough to influence decisions or actions. |
| **Relevance** | Tailor content to the audience’s mission, not the analyst’s interest. |
| **Accuracy** | Verify sources and confidence levels before sharing. |
| **Clarity** | Use clear, concise, jargon-free language. |
| **Security** | Classify and label intelligence appropriately (TLP, internal, etc.). |

---

## 🧠 2. Audience Segmentation

| Audience | Intelligence Type | Format / Example |
|-----------|------------------|------------------|
| **Executives / Management** | Strategic | High-level reports, threat trends, risk summaries |
| **Security Operations / IR Teams** | Tactical | IoCs, TTPs, detection opportunities |
| **Engineering / IT Teams** | Operational | Vulnerability reports, patch priorities |
| **Partners / ISACs / Communities** | Shared Threat Data | STIX/TAXII feeds, community bulletins |

> Before publishing, ask: “Who will act on this intelligence, and how?”

---

## 🗂️ 3. Intelligence Product Types

| Type | Description | Typical Frequency |
|------|--------------|------------------|
| **Flash Alerts** | Immediate warnings on active threats or campaigns. | As needed |
| **Weekly Summaries** | Key events, trends, and vulnerabilities. | Weekly |
| **Threat Actor Profiles** | Deep-dive on a group’s motives, TTPs, and history. | Monthly or quarterly |
| **Campaign Reports** | Analysis of specific intrusion sets or malware families. | As discovered |
| **Strategic Assessments** | Long-term trends, sectoral risk, geopolitical analysis. | Quarterly or annual |

---

## 🌐 4. Sharing Mechanisms

### STIX & TAXII

- **STIX (Structured Threat Information eXpression)**: standardized format for CTI.  
- **TAXII (Trusted Automated eXchange of Indicator Information)**: transport protocol for sharing STIX.

| Use Case | Format | Example |
|-----------|---------|----------|
| Automated IOC sharing | STIX 2.1 over TAXII 2.1 | MISP, ThreatConnect, OpenCTI |
| Human-readable reports | Markdown / PDF | CTI bulletins, intelligence briefs |
| Machine ingestion | JSON feeds | SIEM / SOAR integrations |

> Use **machine-to-machine feeds** for operational data, and **human-readable briefs** for decision-making.

---

## 🔒 5. Classification and Handling (TLP)

| TLP Level | Description | Sharing Scope |
|------------|--------------|----------------|
| **TLP:CLEAR** | Public information; unrestricted. | Internet-wide sharing |
| **TLP:GREEN** | Share within the community or sector. | Peers, ISACs |
| **TLP:AMBER** | Share internally; limited external distribution. | Internal teams, trusted partners |
| **TLP:RED** | Highly sensitive; limited to named recipients only. | Direct individuals |

> Label each report or feed explicitly with its TLP classification and confidence level.

---

## 🔁 6. Feedback Loop

| Feedback Source | Type of Input | Resulting Action |
|------------------|----------------|------------------|
| **SOC / IR Teams** | False positives, gaps, detection outcomes | Refine data sources, improve quality |
| **Executives / Management** | Usefulness of reports, decision support | Adjust content and cadence |
| **Partners / Communities** | External validation, shared context | Enhance correlation and enrichment |

**Feedback channels:**  
- Post-report surveys or forms  
- Periodic intelligence review meetings  
- Metrics: report usage, opened alerts, detections triggered  

---

## 📈 7. Measuring Dissemination Effectiveness

| Metric | Description |
|---------|--------------|
| **Timeliness** | Time between threat emergence and intelligence delivery. |
| **Relevance** | Number of reports that directly influenced decisions or actions. |
| **Engagement** | Feedback received, report opens, alerts followed up. |
| **Quality** | Confidence accuracy, false positive rate. |
| **Coverage** | % of PIRs addressed in intelligence outputs. |

---

## 🧰 8. Best Practices

- Maintain **version control** of intelligence products.  
- Include **confidence scoring** and **data provenance** in every report.  
- Encourage **two-way sharing** with internal and external partners.  
- Establish a **publishing calendar** for regular CTI products.  
- Integrate feedback systematically into the **Direction & Planning phase** of the next cycle.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- FIRST – *Traffic Light Protocol (TLP) v2.0*  
- MITRE – *STIX/TAXII 2.1 Specifications*  
- SANS – *Operationalizing Threat Intelligence Sharing*
