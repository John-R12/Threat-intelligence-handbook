# 🧩 TTP Mapping Guide

**TTP Mapping** connects observed Indicators of Compromise (IoCs) and incidents to **Tactics, Techniques, and Procedures (TTPs)**.  
This provides context on adversary behavior and supports detection, threat hunting, and response.

---

## 🧭 1. Overview

- **Tactics (T)**: The adversary's goals or objectives (the *why*).  
- **Techniques (T)**: How the adversary achieves the tactic (the *how*).  
- **Procedures (P)**: Specific implementations observed in the wild.  

> Mapping IoCs to TTPs helps analysts **understand the attack lifecycle** and anticipate next moves.

---

## ⚙️ 2. Mapping Workflow

1. **Collect Evidence**  
   - Gather IoCs, incident reports, malware samples, network logs.

2. **Identify Adversary Actions**  
   - Look for behavior patterns (e.g., credential dumping, lateral movement, exfiltration).

3. **Select Tactics**  
   - Determine which **tactics** the actions align with (e.g., Persistence, Lateral Movement).

4. **Assign Techniques**  
   - Map observed actions to specific **MITRE ATT&CK techniques** (e.g., T1059 – Command and Scripting Interpreter).

5. **Document Procedures**  
   - Record concrete steps, tools, commands, or scripts used in the incident.

6. **Enrich & Correlate**  
   - Link with prior incidents, campaigns, or known threat actors.  
   - Use internal CTI platforms or feeds for enrichment.

---

## 🧠 3. Example Mapping Table

| IoC / Event | Tactic | Technique (MITRE ATT&CK) | Procedure | Confidence |
|-------------|--------|--------------------------|-----------|------------|
| Suspicious PowerShell | Execution | T1059.001 – PowerShell | PowerShell script downloads malware | High |
| New C2 domain | Command & Control | T1071.001 – Web Protocols | HTTP beaconing to domain | Medium |
| Credential dump | Credential Access | T1003 – OS Credential Dumping | Mimikatz memory dump | High |

> Maintain timestamps, sources, and reference IDs for traceability.

---

## 🕵️‍♂️ 4. Use Cases

1. **Threat Hunting**  
   - Build hypotheses based on TTPs and look for corresponding IoCs in telemetry.

2. **Detection Engineering**  
   - Map coverage gaps in SIEM/EDR alerts by comparing observed TTPs with known techniques.

3. **Campaign Analysis**  
   - Cluster incidents sharing similar TTPs to identify campaigns or threat actors.

4. **Reporting & Communication**  
   - Provide SOC and management with structured, actionable intelligence.

---

## 🧰 5. Best Practices

- Use **consistent TTP naming** (MITRE ATT&CK v12+ recommended).  
- Always include **confidence and source** for each mapping.  
- Update mappings as new evidence or intelligence emerges.  
- Combine with **Diamond Model** for additional relational context.  
- Automate mapping where possible, but validate manually for critical incidents.

---

## 📚 References

- MITRE ATT&CK – *Techniques & TTPs for Enterprise, ICS, and Mobile*  
- SANS – *Practical Threat Intelligence for SOC & IR Teams*  
- NIST SP 800-150 – *Guide to Cyber Threat Information Sharing*  
