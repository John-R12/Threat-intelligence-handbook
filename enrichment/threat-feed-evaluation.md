# 📈 Threat Feed Evaluation Guide

**Threat Feed Evaluation** helps analysts **assess, prioritize, and integrate threat intelligence feeds** to ensure relevance, quality, and operational effectiveness.

---

## 🧩 1. Objectives

- Identify the **most reliable and relevant feeds** for your environment.  
- Evaluate **quality, timeliness, and coverage**.  
- Optimize ingestion into SIEM, SOAR, or CTI platforms.  
- Reduce **noise and false positives** in detection workflows.

---

## ⚙️ 2. Evaluation Criteria

| Criterion | Description | Example Questions |
|-----------|-------------|-----------------|
| **Relevance** | Does the feed contain indicators affecting your sector, assets, or geography? | Are IoCs aligned with your critical systems? |
| **Accuracy / Reliability** | Are indicators verified and attributed correctly? | Are false positives minimal? |
| **Timeliness** | How quickly are new indicators published after discovery? | Are feeds updated in near real-time? |
| **Coverage** | Does the feed cover required threat types (malware, phishing, APTs)? | Does it include TTPs relevant to your environment? |
| **Format / Automation** | Are IoCs available in machine-readable formats? | STIX/TAXII, CSV, JSON, API access? |
| **Cost / Licensing** | Are there financial or legal restrictions? | Commercial vs. open-source; redistribution rights |
| **Integration Ease** | Can the feed be easily ingested into your tools? | SIEM connector availability, API documentation |

---

## 🧠 3. Scoring Feeds

Use a scoring model to prioritize feeds:

| Feed | Relevance | Accuracy | Timeliness | Coverage | Integration | Score |
|------|-----------|---------|------------|----------|-------------|-------|
| Feed A | High | Medium | High | Medium | High | 8/10 |
| Feed B | Medium | High | Medium | High | Medium | 7/10 |
| Feed C | Low | Medium | Low | Low | Medium | 4/10 |

> Define thresholds for **mandatory vs optional feeds** based on operational needs.

---

## 🔄 4. Operational Workflow

1. **Collect Feed Metadata**  
   - Source, type, format, update frequency, cost, licensing.

2. **Test Feed Quality**  
   - Validate IoCs against internal telemetry or historic incidents.

3. **Integrate into CTI Platform**  
   - Configure ingestion pipelines for automated parsing and correlation.

4. **Continuous Monitoring**  
   - Track feed performance: accuracy, latency, false positives.

5. **Periodic Review**  
   - Reassess feeds quarterly or after major incidents.

---

## 🧰 5. Best Practices

- Use a **mix of open-source and commercial feeds**.  
- Prioritize feeds with **machine-readable formats** and structured TTP mappings.  
- Document feed performance and **feedback from SOC/IR teams**.  
- Avoid overloading your platform; focus on **high-value indicators**.  
- Maintain **source attribution** for every IOC ingested.

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- SANS – *Practical Threat Intelligence for SOC Teams*  
- MISP Project – *Threat Feed Management & Evaluation*  
- MITRE ATT&CK – *Mapping Indicators to TTPs*
