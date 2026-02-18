<!-- Header -->
<div align="center">

```
╔═══════════════════════════════════════════════════════════════╗
║          AHMADOU N'DIAYE  //  BLUE TEAM ANALYST               ║
║          DFIR  •  THREAT HUNTING  •  DETECTION ENGINEERING    ║
╚═══════════════════════════════════════════════════════════════╝
```

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0072b1?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmadoundiaye)
[![GitHub](https://img.shields.io/badge/GitHub-333333?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Amadoundiay)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@ndiayeahmadou911)

</div>

---

## 👤 Who I Am

I'm a **Cybersecurity Engineering student** training to operate at the intersection of **DFIR, threat hunting, and detection engineering**.

I don't just complete labs — I investigate them. I reconstruct attacker behavior end-to-end, map findings to **MITRE ATT&CK**, and write reports the way a real IR team would. Every investigation is an opportunity to understand *why* something worked, *how* a defender could have caught it earlier, and *what* detection logic should exist to prevent it from happening again.

My analytical approach is shaped by studying real-world IR reports from **DFIR Report, Mandiant, and Microsoft IR** — and pushing myself to meet that standard in my own work.

> *"Strong defense starts with understanding the attacker — and ends with better detection."*

---

## 🧭 Philosophy

```
  LOG FIRST.       Not assumptions.
  RECONSTRUCT.     Behavior, not just indicators.
  DETECT.          What, when, and how — not just if.
  COMMUNICATE.     Technical precision, executive clarity.
```

Security is not about tools. It's about **visibility, context, and decision-making under pressure**. I train to operate under that pressure before I'm ever put in that position professionally.

---

## 🛡️ Core Capabilities

| Domain | Skills |
|---|---|
| **Threat Detection** | Suricata, YARA, Snort rules, custom Splunk detections |
| **SIEM & Log Analysis** | Splunk, Microsoft Sentinel, Wazuh, KQL |
| **Endpoint & AD Security** | Sysmon, LimaCharlie, Active Directory forensics |
| **DFIR & IR** | Timeline reconstruction, IOC scoping, attacker tradecraft analysis |
| **SOAR & Automation** | Shuffle playbooks, enrichment pipelines |
| **Threat Modeling** | MITRE ATT&CK Framework mapping |
| **Cloud Security** | Microsoft Sentinel, Defender for Cloud |
| **Scripting** | Python, Bash, PowerShell |

---

<br/>

# 🔬 LABS
> *Controlled environments built to simulate real attacker behavior and develop detection muscle memory.*

---

### 🧪 Lab 01 — Phishing Investigation
📋 **[Read Full Lab Report →](https://www.notion.so/Phishing-Investigation-2f0169bd8bbf80319184c52f0244ef35)**

A structured investigation into a phishing-originated intrusion chain. Rather than simply identifying the malicious email, I traced the full post-delivery execution path — from initial payload detonation through persistence mechanisms — documenting every observable artifact and detection opportunity along the way.

**Key focus areas:**
- Email artifact analysis and header forensics
- Payload behavior and process chain reconstruction  
- Detection rule development from observed TTPs
- MITRE ATT&CK mapping across the kill chain

---

### 🧪 Lab 02 — Business Email Compromise (BEC) Investigation
📋 **[Read Full Lab Report →](https://www.notion.so/Business-Email-Compromise-Investigation-300169bd8bbf80d09d62fe6362f561a4)**

BEC attacks are among the most financially damaging — and the most detection-resistant. This investigation focuses on the subtlety of BEC tradecraft: identity manipulation, trust abuse, and low-noise lateral movement that blends seamlessly into legitimate business traffic.

**Key focus areas:**
- Identity-based threat detection without traditional IOCs
- Mailbox rule abuse and account takeover forensics
- Distinguishing attacker behavior from legitimate user activity
- Constructing a coherent timeline from sparse, low-signal artifacts

---

<br/>

# 🚨 INCIDENT REPORTS
> *Real-scenario, DFIR-grade investigations written to the standard of professional IR publications.*

---

### 📁 Incident Report — *"Paging Dr. Warlock"*
### Reconstruction of a Real-World Active Directory Compromise

📋 **[Read Full Incident Report →](https://www.notion.so/Paging-Dr-Warlock-Reconstruction-of-a-Real-World-Active-Directory-Compromise-Featuring-Stealthy--2ee169bd8bbf80f6b7fcd4c67aa76ad2)**

> *Multi-actor. Multi-stage. Stealthy. This is what a real domain compromise looks like.*

This is my most comprehensive investigation to date — a deep forensic reconstruction of a sophisticated Active Directory compromise that unfolded in layers. What made this case exceptional was not just the initial breach, but the **identity theft mechanics** employed by the threat actor: renaming a legitimate account to "Administrator" while quietly demoting the real Administrator, creating a persistent foothold that blended into normal AD noise.

**What I uncovered:**
- **41 correlated alerts** analyzed and attributed across the attack timeline
- Full **domain controller compromise** with multiple backdoor mechanisms
- Evidence of **access being sold to a secondary threat actor** — a hallmark of access broker operations
- Identity manipulation techniques that evaded standard detection logic
- Complete attack chain reconstruction using **Logon ID correlation** across Windows Event IDs 4624, 4648, 4768, and 4776
- Attribution of lateral movement via **SMB and PsExec-style execution**

**Report structure mirrors real-world IR deliverables:**
- Executive Summary
- Attack Timeline (hour-by-hour)
- Phase-by-Phase Technical Analysis
- IOC Scoping & Indicator List
- Detection Gaps & Engineering Opportunities
- MITRE ATT&CK Technique Mapping

This report demonstrates **how I think as an analyst** — not just how I solve challenges.

---

<br/>

# 🏗️ INFRASTRUCTURE & TOOLING PROJECTS

---

### 🖥️ Active Directory Security Lab
📂 [Repository](https://github.com/Amadoundiay/Active-Directory-Project)

Built a realistic Windows Active Directory environment from scratch to simulate attacker behavior from the defender's perspective. Designed for visibility, not just exploitation — every attack simulated was paired with detection logic.

Covered: credential abuse, lateral movement, privilege escalation, Splunk detections mapped to MITRE ATT&CK.

---

### ☁️ Azure Sentinel SOC Lab
📂 [Repository](https://github.com/Amadoundiay/Azure-Sentinel-SOC-Lab)

Cloud-native SOC environment built on Microsoft Sentinel. Deployed a live honeypot to collect real attack telemetry, wrote custom KQL hunting queries, and produced SOC-style investigation reports with attack visualizations and enrichment pipelines (GeoIP, WHOIS, reverse DNS).

---

### 🤖 SOC Automation & Endpoint Telemetry Pipeline

Centralized Sysmon telemetry into Wazuh with automated triage via Shuffle SOAR. Detected credential dumping, suspicious process chains, and lateral movement patterns — reducing analyst alert fatigue through structured workflow-driven response.

> Objective: explore how automation *supports* analysts, not replaces them.

---

<br/>

## ✍️ Technical Writing

I publish security write-ups on **[Medium](https://medium.com/@ndiayeahmadou911)** — covering SOC methodology, threat hunting logic, detection engineering, and lessons learned from real investigations.

Writing is part of the discipline. If I can't explain it clearly, I don't understand it well enough yet.

---

## 📜 Certifications

- 🛡️ **(ISC)² Certified in Cybersecurity (CC)**
- 🌐 **Cisco CCNA – Routing & Switching**
- 🖥️ **TryHackMe SOC Level 1**
- 🛠️ **CompTIA Security+ *(In Progress)***

---

## 🎯 What I'm Looking For

I'm actively seeking **SOC Analyst internships** and **DFIR / Blue Team opportunities** where I can contribute real investigative work — not just ticket triage.

Long-term trajectory: **SOC Tier 2 → DFIR → Detection Engineering**.

📩 Reach me on **[LinkedIn](https://www.linkedin.com/in/ahmadoundiaye)** — let's talk.

---

<div align="center">

*Built from scratch. Investigated with discipline. Written with precision.*

</div>
