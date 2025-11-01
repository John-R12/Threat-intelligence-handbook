# 🧠 IOC Analysis Guide

This guide explains how to **analyze Indicators of Compromise (IoCs)** to determine relevance, context, and actionable insights.

---

## 🧩 1. What is an IOC?

An **Indicator of Compromise (IOC)** is any observable artifact that suggests a system has been or is being compromised.

| Type | Examples |
|------|----------|
| **File-based** | Hashes (MD5, SHA1, SHA256), malware samples |
| **Network-based** | IP addresses, domains, URLs, C2 channels |
| **Host-based** | Registry changes, unusual processes, scheduled tasks |
| **Email-based** | Phishing subjects, sender addresses, malicious attachments |

---

## ⚙️ 2. IOC Analysis Workflow

1. **Collection**  
   - Gather IoCs from internal logs, threat feeds, or incident reports.

2. **Validation**  
   - Verify IoCs for accuracy: check hash values, domains, IPs, and timestamps.  
   - Remove false positives or obsolete indicators.

3. **Contextualization**  
   - Determine associated threat actors, TTPs, campaigns.  
   - Map IoCs to MITRE ATT&CK techniques or Diamond Model components.

4. **Prioritization**  
   - Assign a **criticality level** based on potential impact and likelihood.  
   - Consider business-critical assets affected.

5. **Enrichment**  
   - Add intelligence from external sources: threat feeds, sandbox analysis, WHOIS data, passive DNS.

6. **Documentation**  
   - Maintain structured records with confidence, source, and timestamp.  
   - Use standardized formats: STIX, CSV, or your CTI platform.

---

## 🧭 3. IOC Scoring and Confidence

| Metric | Description |
|--------|-------------|
| **Confidence** | High, Medium, Low — reliability of the source and validation. |
| **Relevance** | How applicable the IOC is to your environment. |
| **Recency** | How recent the indicator was observed in the wild. |
| **Impact** | Potential damage if IOC is realized. |

> Example: A SHA256 hash observed in a targeted phishing campaign affecting finance systems → High confidence, High relevance.

---

## 🕵️‍♂️ 4. Correlation and Context

- Correlate IoCs with **internal alerts** and prior incidents.  
- Identify **common infrastructure** across multiple IoCs (e.g., C2 servers).  
- Map to **adversary profiles** to determine tactics and potential next moves.

---

## 🧰 5. Tools and Techniques

| Task | Tools / Methods |
|------|----------------|
| Hash analysis | VirusTotal, Hybrid Analysis, Cuckoo Sandbox |
| Domain/IP investigation | Passive DNS, WHOIS, ThreatCrowd, AbuseIPDB |
| Threat actor mapping | MITRE ATT&CK, Diamond Model, Campaign Reports |
| IOC enrichment | MISP, OpenCTI, internal CTI platforms |

> Automation is encouraged but manual validation ensures accuracy.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- MITRE ATT&CK – *Techniques & Threat Actor Mapping*  
- SANS – *Practical Threat Intelligence for SOC Teams*  
- MISP Project – *Indicators Management & Correlation*
