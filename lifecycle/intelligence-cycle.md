# 🔁 Cyber Threat Intelligence Lifecycle

The **Cyber Threat Intelligence (CTI) lifecycle** is a structured process for planning, collecting, analyzing, and sharing intelligence.  
It ensures that intelligence activities are focused, repeatable, and aligned with organizational goals.

---

## 🧩 The Six Phases

| Phase | Description | Key Deliverables |
|:------|:-------------|:-----------------|
| **1. Direction (Planning & Requirements)** | Define intelligence objectives based on business, security, or operational needs. Prioritize what intelligence is required and why. | Intelligence Requirements (PIRs), Collection Plan |
| **2. Collection** | Gather data from relevant sources: internal telemetry, open-source, dark web, and commercial feeds. | Raw Data, IoCs, Threat Reports |
| **3. Processing** | Clean, normalize, and structure collected data for analysis. | Parsed & Structured Datasets |
| **4. Analysis** | Correlate, validate, and interpret processed data to extract meaning and assess threat relevance. | Intelligence Assessments, TTP Mapping, Adversary Profiles |
| **5. Dissemination** | Deliver the intelligence product to stakeholders in a clear and actionable format. | Reports, Alerts, Dashboards, Briefings |
| **6. Feedback** | Gather stakeholder feedback to refine requirements, improve relevance, and close the intelligence loop. | Updated Requirements, Lessons Learned |

---

## 🧭 1. Direction – Defining Requirements
The foundation of all intelligence work is **asking the right questions**.  
Define what decisions need to be supported by intelligence.

**Examples of Priority Intelligence Requirements (PIRs):**
- Which threat actors are most likely to target our sector?
- What tactics and tools are they currently using?
- What vulnerabilities are being exploited in the wild?

🧱 *Output:* Collection Plan, Intelligence Objectives, and Stakeholder Alignment.

---

## 🌐 2. Collection – Gathering Data
Collect data from multiple, reliable sources:

- Internal logs, alerts, incident reports  
- OSINT feeds and community repositories  
- Commercial or government threat feeds  
- Dark web monitoring and forums  

📦 *Output:* Raw threat data and contextual indicators.

---

## ⚙️ 3. Processing – Structuring the Data
Collected data must be **normalized, enriched, and deduplicated** before analysis.  
Typical actions include:
- Parsing and converting formats (STIX, CSV, JSON)
- Tagging indicators with metadata (confidence, source, date)
- Filtering noise and duplicates
- Correlating related IoCs

🔧 *Output:* Cleaned, structured, enriched datasets.

---

## 🧠 4. Analysis – Making Sense of the Data
The goal is to **transform information into intelligence**.  
Analysts interpret the data to understand threats, motives, and potential impact.

**Key methods:**
- Pattern correlation and clustering  
- Mapping to **MITRE ATT&CK TTPs**  
- Applying frameworks such as the **Diamond Model** or **Kill Chain**  
- Evaluating confidence and reliability  

📊 *Output:* Intelligence assessments, actor profiles, TTP maps.

---

## 📢 5. Dissemination – Delivering Intelligence
Intelligence has value only when **shared with the right audience** in time.  
Deliver tailored outputs depending on your stakeholders:
- **Executives:** concise threat briefings  
- **SOC/IR teams:** operational IoCs, TTPs  
- **IT teams:** vulnerability prioritization  
- **Partners:** collaborative intelligence via STIX/TAXII  

🗂️ *Output:* Reports, dashboards, alerts, or data feeds.

---

## 🔄 6. Feedback – Continuous Improvement
Feedback ensures your CTI program evolves effectively.  
Collect input from stakeholders about:
- Relevance and accuracy of intelligence  
- Format and timing of deliverables  
- Gaps in coverage or new requirements  

🔁 *Output:* Refined intelligence priorities, improved processes, stronger collaboration.

---

## 🧩 Summary Diagram
[Direction] → [Collection] → [Processing] → [Analysis] → [Dissemination] → [Feedback]

---

## 🧰 Best Practices
- Keep intelligence **goal-driven**, not data-driven.  
- Document **sources, confidence, and assumptions**.  
- Maintain traceability from **requirement → analysis → output**.  
- Review and refine your lifecycle at least quarterly.  

---

## 📚 References
- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- ENISA – *Cyber Threat Intelligence Framework*  
- SANS – *Practical Guide to Cyber Threat Intelligence*  
- MITRE ATT&CK – *Adversary Tactics and Techniques Knowledge Base*
