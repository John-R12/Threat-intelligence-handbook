# 🧠 Threat Intelligence Handbook

The **Threat Intelligence Handbook** provides a structured, practical guide for building and operating a **Cyber Threat Intelligence (CTI)** capability.  
It is designed for analysts, SOCs, CERTs, and defenders who want to collect, analyze, and apply intelligence effectively.

---

## 🎯 Purpose
This repository helps you:
- Understand and apply the **Threat Intelligence lifecycle**.
- Identify and evaluate intelligence sources (open, dark, commercial).
- Analyze indicators, adversary campaigns, and TTPs.
- Share intelligence securely and efficiently (STIX, TAXII, TLP).
- Enrich and score data to improve operational value.
- Apply CTI frameworks and standards for structured analysis.

---

## 📂 Repository Structure

| Folder | Description |
|--------|--------------|
| `lifecycle/` | Defines the CTI lifecycle, collection plans, and analytical frameworks. |
| `sources/` | Catalogs and evaluates intelligence feeds and data sources. |
| `analysis/` | Provides methods and templates for IoC, TTP, campaign, and threat-hunting analysis. |
| `enrichment/` | Details enrichment techniques, pivoting, and scoring models. |
| `sharing/` | Covers intelligence sharing models, communication templates, and feedback mechanisms. |
| `frameworks/` | Provides CTI frameworks (MITRE ATT&CK, Diamond Model, Kill Chain) and standards (STIX/TAXII, MISP). |

---

## 🧩 How to Use
1. Start with [`lifecycle/intelligence-cycle.md`](./lifecycle/intelligence-cycle.md) to understand the CTI process.  
2. Explore `sources/` to identify data feeds and evaluate their reliability.  
3. Use `analysis/` to structure your analytical process and conduct threat hunting.  
4. Apply `sharing/` templates for reporting, internal/external communication, and feedback loops.  
5. Leverage `enrichment/` to enhance your data and intelligence output.  
6. Reference `frameworks/` to map TTPs, structure campaigns, and ensure standardized reporting.

---

## 📚 References
- [NIST SP 800-150](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-150.pdf) — *Guide to Cyber Threat Information Sharing*  
- [ENISA Threat Intelligence Framework](https://www.enisa.europa.eu/publications/strategic-intelligence-framework)  
- [MITRE ATT&CK](https://attack.mitre.org/)  
- [FIRST Traffic Light Protocol (TLP)](https://www.first.org/tlp/)

---

## 🤝 Contributing
Contributions are welcome!  
To propose new content:
- Follow the style and tone of existing markdowns.  
- Ensure neutrality (no vendor-specific content).  
- Reference trusted, public sources.

---

## ⚠️ Disclaimer
This repository provides **generic and educational guidance**.  
Adapt all content to your organization’s specific context, tools, and legal framework.
