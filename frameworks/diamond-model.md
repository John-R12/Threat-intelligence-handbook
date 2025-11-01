# 💎 Diamond Model of Intrusion Analysis

The **Diamond Model** is a framework for understanding and analyzing cyber intrusions by visualizing the relationships between core components of an attack.  
It is widely used in CTI for **campaign clustering, attribution, and correlation**.

---

## 🧩 1. Core Components

| Component | Description | Example |
|-----------|-------------|---------|
| **Adversary** | Entity responsible for the intrusion (individual, group, nation-state). | APT29, FIN7 |
| **Capability** | Tools, malware, or techniques used to execute the attack. | Cobalt Strike, PowerShell scripts |
| **Infrastructure** | Systems, networks, or services leveraged by the adversary. | Compromised VPS, C2 domains, phishing infrastructure |
| **Victim** | Targeted organization, sector, or individual. | Financial institution, healthcare provider |

> Each intrusion is represented as a **diamond**, with the components forming the vertices.

---

## ⚙️ 2. Relationships

The **edges of the diamond** represent the interactions between components:

| Edge | Meaning |
|------|---------|
| Adversary → Capability | Who is using what tool or malware. |
| Capability → Infrastructure | How tools are deployed through infrastructure. |
| Infrastructure → Victim | Which victims are affected by the infrastructure. |
| Victim → Adversary | Feedback loop: attack detection leads to further intelligence. |

These relationships help identify **shared capabilities or infrastructure** across multiple attacks, supporting attribution and campaign analysis.

---

## 🕵️‍♂️ 3. Use Cases in CTI

1. **Campaign Correlation**  
   - Identify when multiple incidents share the same adversary, infrastructure, or malware.  
   - Example: Two ransomware campaigns using the same C2 servers may be linked.

2. **Adversary Profiling**  
   - Characterize threat actors by their techniques and targets.  
   - Supports prioritization and mitigation planning.

3. **Threat Hunting & Detection**  
   - Generate hypotheses for hunts based on observed patterns.  
   - Map detected IoCs to the diamond components.

4. **Reporting & Communication**  
   - Provide structured visualization of attacks to SOC, IR, or executives.

---

## 📊 4. Example Diagram

      [ Adversary ]
          /    \
 [ Capability ] [ Infrastructure ]
          \    /
         [ Victim ]

- Each edge can be annotated with **time, confidence, and evidence**.  
- Multiple diamonds can be connected to map a **campaign or attack cluster**.

---

## 🧰 5. Best Practices

- Always record **evidence for each edge** (logs, malware samples, network traffic).  
- Assign **confidence levels** to each component and relationship.  
- Combine with **MITRE ATT&CK** for standardized TTP mapping.  
- Use visualization tools to manage complex multi-diamond analyses.

---

## 📚 References

- Caltagirone, Pendergast & Betz – *The Diamond Model of Intrusion Analysis*, 2013  
- SANS CTI Summit – *Applying Diamond Model in Operational Threat Intelligence*  
- MITRE ATT&CK – *Integration with Diamond Model for Threat Analysis*
