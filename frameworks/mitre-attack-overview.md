# 🧩 MITRE ATT&CK Framework Overview

The **MITRE ATT&CK Framework** (Adversarial Tactics, Techniques & Common Knowledge) is a globally recognized model for understanding, categorizing, and mapping adversary behaviors.

It provides a structured way to **analyze cyber threats**, **develop detections**, and **measure defense coverage**.

---

## 🧭 1. Purpose

The MITRE ATT&CK framework was created to:
- Document **real-world adversary behaviors** observed in the wild.
- Provide a **common language** for describing tactics and techniques.
- Help security teams **detect, defend, and respond** more effectively.
- Enable **threat-informed defense** across organizations.

---

## 🧠 2. Structure of ATT&CK

ATT&CK is organized hierarchically:

| Level | Description | Example |
|--------|--------------|---------|
| **Tactic** | The adversary’s technical objective (the "why"). | *Persistence* |
| **Technique** | How the objective is achieved (the "how"). | *T1059 – Command and Scripting Interpreter* |
| **Sub-technique** | A specific implementation or variation. | *T1059.003 – Windows Command Shell* |
| **Procedure** | A concrete instance observed in the wild. | *APT29 using PowerShell for lateral movement* |

---

## 🧩 3. ATT&CK Matrices

MITRE ATT&CK is divided into multiple **matrices** depending on the environment:

| Matrix | Focus | Example Use |
|---------|--------|-------------|
| **Enterprise** | Tactics and techniques in Windows, Linux, macOS, and cloud environments. | Detection & hunting |
| **Mobile** | Techniques targeting iOS and Android. | Mobile threat analysis |
| **ICS** | Industrial Control Systems environments. | OT/critical infrastructure protection |

---

## ⚙️ 4. Tactics Overview (Enterprise)

| ID | Tactic | Description |
|----|---------|--------------|
| TA0001 | Initial Access | How adversaries first gain access to systems. |
| TA0002 | Execution | Running malicious code on a system. |
| TA0003 | Persistence | Maintaining foothold. |
| TA0004 | Privilege Escalation | Gaining higher-level permissions. |
| TA0005 | Defense Evasion | Avoiding detection and mitigation. |
| TA0006 | Credential Access | Stealing account credentials. |
| TA0007 | Discovery | Understanding the environment. |
| TA0008 | Lateral Movement | Moving through the network. |
| TA0009 | Collection | Gathering data of interest. |
| TA0010 | Exfiltration | Removing data from the environment. |
| TA0040 | Impact | Manipulating, interrupting, or destroying systems/data. |

---

## 🕵️ 5. ATT&CK in Threat Intelligence

ATT&CK enables CTI analysts to:
- Map observed TTPs in incident reports to a **standard vocabulary**.  
- Track **adversary evolution** over time.  
- Compare **actor profiles** across campaigns.  
- Support **detection engineering** and **hunt hypotheses**.

Example:

> "Adversary used PowerShell (T1059.001) to execute malicious scripts during lateral movement (TA0008)."

---

## 🧰 6. ATT&CK in Practice

### Use Cases
- **Threat Intelligence Correlation:** Align actor behaviors with known groups.  
- **Detection Engineering:** Validate coverage using ATT&CK Navigator.  
- **SOC Metrics:** Measure detection coverage by tactic.  
- **Hunt Development:** Form hypotheses from common techniques.  

### Common Tools
- [MITRE ATT&CK Navigator](https://attack.mitre.org/resources/navigator/)  
- [ATT&CK Workbench](https://github.com/mitre-attack/attack-workbench)  
- [ATT&CK CTI Mappings](https://github.com/mitre-attack/attack-cti)  

---

## 🔄 7. Maintaining ATT&CK Mappings

- Review and update mappings **quarterly**.  
- Record **confidence level** for each technique attribution.  
- Use **STIX 2.1 objects** for structured representation.  
- Maintain **traceability** between reports, actors, and mapped TTPs.

---

## 📚 References
- [MITRE ATT&CK – Official Website](https://attack.mitre.org/)  
- [MITRE ATT&CK Navigator](https://mitre-attack.github.io/attack-navigator/)  
- *Threat-Informed Defense: Applying MITRE ATT&CK to Cyber Threat Intelligence (MITRE Engenuity, 2020)*  
- *SANS CTI Summit: Mapping Threat Reports to ATT&CK*  
