# ⚔️ Cyber Kill Chain (Lockheed Martin)

The **Cyber Kill Chain** is a framework developed by Lockheed Martin to **model the stages of a cyber attack**.  
It is widely used in threat intelligence, SOC operations, and red/blue team exercises to **understand, detect, and disrupt adversary activity**.

---

## 🧩 1. Kill Chain Phases

| Phase | Description | Detection / Defense Focus |
|-------|-------------|---------------------------|
| **1. Reconnaissance** | Adversary gathers information about targets, employees, systems, or vulnerabilities. | OSINT monitoring, phishing awareness, perimeter monitoring |
| **2. Weaponization** | Creating a deliverable (malware, exploit) tailored to the target. | Malware sandboxing, threat feed correlation |
| **3. Delivery** | Transmission of weaponized payload to the target (email, web, USB). | Email filtering, web proxy controls, DLP |
| **4. Exploitation** | Executing the payload to gain initial access. | Endpoint protection, vulnerability patching |
| **5. Installation** | Establishing persistence in the environment. | EDR monitoring, IOC detection |
| **6. Command & Control (C2)** | Connecting to attacker infrastructure for instructions. | Network monitoring, firewall/IDS rules, anomaly detection |
| **7. Actions on Objectives** | Completing the attack goals: exfiltration, encryption, sabotage, etc. | DLP, backups, incident response, forensic analysis |

> Note: Modern attacks may skip phases or iterate in loops. Always consider **non-linear attacks**.

---

## 🧠 2. Applications in Threat Intelligence

1. **Detection Gap Analysis**  
   - Map observed incidents to kill chain phases to identify missing controls.  

2. **Threat Hunting**  
   - Develop hypotheses based on likely next steps of attackers in current campaigns.  

3. **Red Team & Blue Team Exercises**  
   - Use the chain to simulate attacks and test defenses.  

4. **Reporting & Communication**  
   - Provide structured analysis for management and stakeholders.

---

## 🔄 3. Integration with Other Frameworks

| Framework | Integration Use Case |
|-----------|--------------------|
| **Diamond Model** | Map adversary, capability, infrastructure, and victim per phase. |
| **MITRE ATT&CK** | Map detected techniques to kill chain stages for standardized reporting. |
| **STIX/TAXII** | Share kill chain-based indicators with partners in structured format. |

> Combining frameworks improves **contextual awareness, correlation, and defensive planning**.

---

## 📊 4. Visual Example

[Recon] → [Weaponize] → [Deliver] → [Exploit] → [Install] → [C2] → [Actions on Objectives]

- Each phase can be annotated with **IoCs, TTPs, evidence, and confidence**.  
- Use for mapping multiple incidents or campaigns to identify patterns.

---

## 🧰 5. Best Practices

- Keep the chain **dynamic**; attacks may not follow strict linear steps.  
- Map **observed TTPs** to each phase for SOC dashboards and hunting exercises.  
- Include **mitigation and detection controls** for each phase.  
- Review **lessons learned** from past incidents to refine the chain application.

---

## 📚 References

- Lockheed Martin – *Intelligence-Driven Computer Network Defense* (2011)  
- SANS Institute – *Cyber Threat Intelligence Summit Materials*  
- MITRE ATT&CK – *Mapping TTPs to Kill Chain Phases*  
