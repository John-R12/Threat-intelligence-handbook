# 📊 Campaign Tracking Guide

**Campaign Tracking** in Cyber Threat Intelligence (CTI) involves **grouping related incidents, IoCs, and TTPs** to identify ongoing campaigns and threat actor activity.  
This allows organizations to **prioritize defenses, anticipate adversary behavior, and improve situational awareness**.

---

## 🧩 1. Objectives

- Identify patterns and connections between incidents.  
- Attribute incidents to specific threat actors or groups.  
- Track adversary TTP evolution over time.  
- Support threat hunting and detection coverage assessment.

---

## ⚙️ 2. Campaign Tracking Workflow

1. **Collect Incident Data**  
   - Gather all relevant incidents, IoCs, TTP mappings, and contextual intelligence.

2. **Normalize Data**  
   - Ensure consistent formats, timestamps, and metadata.  
   - Tag with confidence levels, sources, and environment relevance.

3. **Cluster Related Events**  
   - Group incidents sharing:
     - Same **TTPs**
     - Shared **infrastructure** (IP, domains, C2 servers)
     - Similar **malware or toolsets**
     - Overlapping **targets or sectors**

4. **Analyze Campaign Attributes**  
   - Determine likely adversary, motivation, and objectives.  
   - Track geographic and temporal patterns.

5. **Document & Visualize**  
   - Create dashboards, timelines, or network graphs showing campaign relationships.  
   - Include key IoCs, TTPs, and known actor profiles.

6. **Update Continuously**  
   - Incorporate new incidents or intelligence as they occur.  
   - Refine clustering and attribution.

---

## 🧠 3. Example Campaign Table

| Campaign | Incident IDs | Key TTPs | Infrastructure | Threat Actor | Status |
|----------|--------------|----------|----------------|--------------|--------|
| Ransomware-Financial-Q4 | IR-2025-01, IR-2025-03 | T1486 – Data Encrypted for Impact, T1059 – Command Interpreter | Malicious domains, compromised VPS | FIN7 | Active |
| Phishing-Executive-2025 | IR-2025-04, IR-2025-05 | T1566 – Phishing, T1071 – Application Layer Protocol | Email servers, phishing domains | APT29 | Active |

> Include **source, confidence, and last observed date** for traceability.

---

## 🔄 4. Integration with TTP Mapping & IOC Analysis

- Campaign tracking **builds on IoC analysis and TTP mapping**:
  - IoCs → mapped to TTPs → clustered by campaign.  
- This enables proactive **threat hunting** and **detection engineering**:
  - E.g., if a TTP appears in multiple campaigns, prioritize detection rules.

---

## 🧰 5. Tools & Techniques

| Task | Tools / Techniques |
|------|-------------------|
| Data aggregation | SIEM, CTI platform, MISP, OpenCTI |
| Visualization | Kibana, Grafana, Maltego, Gephi |
| Campaign clustering | Graph databases, link analysis, Excel/Sheets |
| Attribution support | Diamond Model, MITRE ATT&CK, threat reports |

---

## 🧰 6. Best Practices

- Maintain **consistent naming conventions** for campaigns and incidents.  
- Track **confidence levels** for each attribution.  
- Regularly **review and refine clusters** based on new evidence.  
- Document **decision rationale** for each campaign link.  
- Integrate campaign tracking with **SOC dashboards and hunting playbooks**.

---

## 📚 References

- SANS – *Practical Threat Intelligence for SOC & IR Teams*  
- MITRE – *ATT&CK Campaign Mapping Guidance*  
- Caltagirone, Pendergast & Betz – *Diamond Model of Intrusion Analysis*  
- ENISA – *Threat Intelligence Guidelines for Critical Infrastructure*
