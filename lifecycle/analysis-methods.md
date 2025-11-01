# 🧠 Threat Intelligence Analysis Methods

Analysis transforms **data** into **intelligence**.  
It connects indicators, behaviors, and context to reveal *who*, *how*, and *why* behind cyber threats.  
This guide presents common analytical frameworks used in Cyber Threat Intelligence (CTI).

---

## 🧩 1. The Diamond Model of Intrusion Analysis

The **Diamond Model** visualizes intrusions through four core components:

| Element | Description | Example |
|----------|--------------|---------|
| **Adversary** | The threat actor or group conducting malicious activity. | APT29, FIN7 |
| **Capability** | Tools, exploits, or malware used by the adversary. | Cobalt Strike, PlugX |
| **Infrastructure** | Systems and services the adversary uses to deliver or control attacks. | Compromised VPS, malicious domains |
| **Victim** | The targeted organization, sector, or individual. | Financial institutions, energy sector |

**Relationships** between these elements form the *edges* of the diamond — mapping how adversaries operate.

**Uses:**
- Correlate related intrusions.
- Identify shared infrastructure or tools.
- Support attribution and clustering.

**Example Diagram:**

              [ Adversary ]
                  /    \
       [ Capability ] [ Infrastructure ]
                  \    /
                [ Victim ]

---

## ⚔️ 2. The Cyber Kill Chain (Lockheed Martin)

The **Kill Chain** describes the sequential phases of an attack, from reconnaissance to objectives.  
It helps identify where defenses can detect or disrupt adversary actions.

| Phase | Description | Defensive Focus |
|-------|--------------|-----------------|
| **1. Reconnaissance** | Gather information about targets. | Threat hunting, OSINT monitoring |
| **2. Weaponization** | Create exploit or payload. | Malware analysis, sandboxing |
| **3. Delivery** | Send payload to the target. | Email/web filtering, WAF |
| **4. Exploitation** | Execute malicious code. | Patch management, endpoint protection |
| **5. Installation** | Establish persistence. | EDR, IOC detection |
| **6. Command & Control (C2)** | Connect to attacker infrastructure. | Network monitoring, proxy filtering |
| **7. Actions on Objectives** | Exfiltration, encryption, sabotage. | DLP, behavioral monitoring |

**Usage in CTI:**
- Map observed TTPs to attack phases.
- Identify defensive gaps.
- Support detection engineering and red team planning.

---

## 🕵️‍♂️ 3. MITRE ATT&CK Framework

**MITRE ATT&CK** provides a global knowledge base of adversary tactics, techniques, and procedures (TTPs).  
It organizes attacks by **Tactic (why)** and **Technique (how)**.

| Layer | Description | Example |
|--------|--------------|---------|
| **Tactics** | The adversary’s objectives (e.g., Initial Access, Execution, Persistence). | *Persistence* |
| **Techniques** | Specific methods used to achieve the tactic. | *T1059 – Command and Scripting Interpreter* |
| **Sub-techniques** | Variants or implementations of a technique. | *T1059.003 – Windows Command Shell* |

**Applications:**
- Standardized threat reporting.
- Mapping detections to known TTPs.
- Measuring coverage and detection maturity.
- Correlating incidents with known threat groups.

> Combine MITRE ATT&CK with internal telemetry to strengthen detection engineering and threat hunting.

---

## 🔍 4. The Intelligence Analysis Process

Beyond frameworks, **analytical rigor** is essential.  
Follow a repeatable approach to ensure objectivity and reliability:

1. **Define the question.**  
   What are we trying to understand or predict?

2. **Collect relevant data.**  
   Logs, IoCs, reports, malware samples, etc.

3. **Assess data quality.**  
   Source reliability, information credibility, confidence level.

4. **Correlate and interpret.**  
   Link indicators, behaviors, and actors.

5. **Apply frameworks.**  
   Diamond Model, Kill Chain, ATT&CK, etc.

6. **Draw conclusions and assess confidence.**  
   Use structured analytic techniques (SATs) like *Analysis of Competing Hypotheses (ACH)*.

---

## 🧩 5. Confidence and Attribution

When presenting intelligence, include a **confidence level** and note **uncertainties**.

| Confidence Level | Meaning |
|------------------|----------|
| **High** | Multiple reliable sources confirm findings. |
| **Medium** | Some supporting evidence; moderate certainty. |
| **Low** | Limited or conflicting information. |

> Use consistent language like *“with high confidence”* or *“with moderate confidence”*.

---

## 🧰 6. Combining Frameworks

Each model offers a unique perspective:

| Framework | Focus | Best Use Case |
|------------|--------|---------------|
| **Diamond Model** | Entity relationships | Clustering campaigns, attribution |
| **Kill Chain** | Attack sequence | Detection gap analysis |
| **MITRE ATT&CK** | Techniques and behavior mapping | Detection engineering, hunt development |

**Example Combined View:**

Diamond Model (Who/What) → Kill Chain (When/How) → MITRE ATT&CK (How Specifically)

---

## 📚 References
- *The Diamond Model of Intrusion Analysis* – Caltagirone, Pendergast & Betz  
- *Intelligence-Driven Computer Network Defense* – Lockheed Martin  
- *MITRE ATT&CK Framework* – https://attack.mitre.org  
- *SANS CTI Summit – Analytic Techniques for Threat Intelligence*  
