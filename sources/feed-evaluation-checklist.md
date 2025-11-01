# ✅ Threat Feed Evaluation Checklist

Use this checklist to **assess the quality and relevance** of threat intelligence feeds before onboarding them into your CTI platform or SOC workflow.

---

## 🧩 Feed Information

| Field | Example |
|--------|----------|
| Feed Name | ExampleFeed.io |
| Provider | Example Security Labs |
| Type | OSINT / Commercial / Sectoral |
| Format | STIX 2.1 / CSV / JSON / TAXII |
| Update Frequency | Hourly / Daily / Weekly |
| Source Reliability | High / Medium / Low |
| Cost | Free / Subscription / Partnership |

---

## ⚙️ Evaluation Criteria

| Criterion | Description | Score (1–5) |
|------------|-------------|-------------|
| **Relevance** | Matches your sector, assets, and geography. |   |
| **Accuracy** | Low false positive rate, validated indicators. |   |
| **Timeliness** | Updates promptly after threat discovery. |   |
| **Coverage** | Broad coverage (malware, phishing, TTPs, APTs). |   |
| **Format & Automation** | Machine-readable and easily integrated. |   |
| **Documentation** | Clear description of data sources and methodology. |   |
| **Support & Responsiveness** | Vendor/community support available. |   |

> **Scoring tip:**  
> - 5 = Excellent, 4 = Good, 3 = Average, 2 = Poor, 1 = Inadequate  
> - Total Score ≥ 30 → Recommended Feed  

---

## 📈 Example Summary

| Feed | Total Score | Decision | Notes |
|------|--------------|----------|-------|
| Feed A | 34 | ✅ Approve | Good coverage and accuracy |
| Feed B | 25 | ⚠️ Review | Needs better documentation |
| Feed C | 17 | ❌ Reject | Outdated indicators |

---

## 🧰 Best Practices

- Document **why** a feed was accepted or rejected.  
- Re-evaluate all feeds **quarterly** or after major incidents.  
- Encourage **feedback from analysts** on feed usefulness.  
- Maintain a **feed inventory** with metadata (contact, license, update rate).  

---

## 📚 References

- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
- MISP Project – *Feed Management Guide*  
- SANS – *Operationalizing Threat Intelligence*  
