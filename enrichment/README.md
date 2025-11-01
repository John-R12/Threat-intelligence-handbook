# 🧪 Threat Intelligence Enrichment

This folder contains documents and guides related to **enriching raw threat data** to make it actionable.  
Enrichment improves the **context, relevance, and usability** of indicators before analysis or sharing.

---

## 🧩 Objectives

- Add context to raw threat data (IPs, domains, hashes, malware samples, etc.).  
- Assign confidence scores and relevance to each indicator.  
- Correlate information with previous incidents or known threat actors.  
- Prepare data for ingestion into **SOC, SIEM, SOAR, or CTI platforms**.

---

## 📁 Files

| File | Description |
|------|-------------|
| [`threat-feed-evaluation.md`](./threat-feed-evaluation.md) | Checklist and methodology for evaluating threat feeds. |
| [`enrichment-playbook.md`](./enrichment-playbook.md) | Step-by-step guidance on enriching indicators with context and metadata. |

---

## ⚙️ How to Use

1. Evaluate each feed using the **Threat Feed Evaluation** checklist.  
2. Apply the **Enrichment Playbook** to add context, classify, and prioritize indicators.  
3. Ensure enriched data is **structured and machine-readable** where needed.  
4. Feed enriched data into the **analysis and dissemination workflow**.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- ENISA – *Good Practices for Threat Intelligence Sharing*  
- MISP Project – *Operationalizing Threat Intelligence Feeds*
