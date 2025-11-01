# 🕵️‍♂️ Dark Web Intelligence Sources

> ⚠️ **Legal & Ethical Disclaimer:**  
> Accessing or collecting data from the dark web must comply with **all applicable laws and organizational policies**.  
> This document focuses on **passive monitoring** and **third-party intelligence acquisition**, not active participation or infiltration.

---

## 🧭 1. Overview

The **Dark Web** hosts underground marketplaces, leak forums, ransomware blogs, and criminal communication channels.  
Monitoring these sources provides valuable insights into:
- Data breaches and credential leaks,  
- Ransomware group announcements,  
- Sale of exploits, malware, or access to systems,  
- Early indicators of planned attacks,  
- Emerging threat actor groups or alliances.  

However, dark web intelligence must be collected **ethically**, **securely**, and **filtered** to avoid exposure or contamination.

---

## 🌐 2. Types of Dark Web Sources

| Type | Description | Access Method |
|------|--------------|----------------|
| **Leak Sites** | Ransomware group “data leak” blogs. | Publicly accessible `.onion` mirrors or scraped feeds. |
| **Marketplaces** | Platforms selling data, credentials, or tools. | Restricted Tor access; mostly monitored by specialized vendors. |
| **Forums & Chats** | Cybercriminal discussion boards (English, Russian, Chinese). | Access-controlled; high OPSEC required. |
| **Paste Sites & Dump Repositories** | Anonymous data pasting/sharing services. | Often indexed by OSINT tools (e.g., Pastebin, Ghostbin). |
| **Telegram & Social Media Channels** | Semi-open groups for selling or sharing breach data. | Requires manual monitoring or API collection. |

---

## 🧰 3. Intelligence Collection Methods

| Method | Description | Notes |
|---------|--------------|-------|
| **Vendor Feeds** | Use trusted third-party dark web monitoring services. | Legal, low risk (e.g., KELA, Intel471, DarkOwl). |
| **Partnerships** | Information exchange with CERTs, law enforcement, or ISACs. | Controlled, contextualized sharing. |
| **Automated Crawlers** | Self-managed crawling for `.onion` or Telegram content. | ⚠️ Use in compliance with legal boundaries. |
| **Manual Monitoring** | Analyst-driven observation of key forums or channels. | Requires strong OPSEC (VPN + Tor + sandbox). |

---

## 🛡️ 4. OPSEC & Security Recommendations

| Category | Best Practice |
|-----------|----------------|
| **Environment Isolation** | Use VMs or sandboxed systems with no internal network access. |
| **Network Hygiene** | Always connect via Tor over VPN or secure proxy. |
| **Identity Protection** | Never use real names, emails, or identifiable handles. |
| **Data Sanitization** | Strip PII and illegal material from collected samples. |
| **Documentation** | Maintain logs of collection and justification for compliance. |

---

## 🧩 5. Integration into CTI Workflows

- Feed dark web alerts into **CTI or SIEM platforms** for correlation.  
- Focus on **indicators and context**, not raw content.  
- Use **automation** for keyword monitoring (brand names, IPs, domains).  
- Link findings to **threat actor profiles** or **campaign tracking** in `analysis/`.  

---

## 📎 6. Recommended Vendors & Tools

| Type | Example Tools / Platforms |
|------|----------------------------|
| **Commercial Dark Web Monitoring** | KELA, Intel471, DarkOwl, Recorded Future, Cybersixgill |
| **Open Source / Community** | OnionSearch, Ahmia, TorBot, Lampyre (limited free tier) |
| **Hybrid / Feed Integrations** | MISP, OpenCTI with dark web connectors |

---

## 🧠 7. Key Takeaways

- Dark web intelligence is **high-value but high-risk**.  
- Always prioritize **legality, safety, and analyst anonymity**.  
- Favor **indirect collection** through trusted intermediaries when possible.  
- Treat all data as **potentially toxic or contaminated** until verified.  

---

## 📚 References

- ENISA – *Dark Web Monitoring for Threat Intelligence*  
- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- Europol – *Dark Web Monitoring Guidelines*  
- MITRE ATT&CK – *Adversary Infrastructure Use*  
