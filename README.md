<div align="center">

# 🔬 SOC-Investigation-Labs

*Threat detection exercises written to analyst standards*

[![Author](https://img.shields.io/badge/Ahmadou%20N'Diaye-0072b1?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/ahmadoundiaye)
[![MITRE](https://img.shields.io/badge/MITRE%20ATT%26CK-mapped-red?style=flat-square)](https://attack.mitre.org)

</div>

---

These are not walkthroughs. Every lab is treated as a real incident — evidence collected, behavior reconstructed, detection gaps documented, and findings written up the way a SOC analyst would hand them to a team lead.

Each report lives on Notion with full technical depth. What's here is the case file.

---

## Labs

### 🧪 Lab 01 — Phishing Investigation
📋 [Full Report →](https://www.notion.so/Phishing-Investigation-2f0169bd8bbf80319184c52f0244ef35)

A user executes a malicious attachment. This investigation doesn't stop at identifying the email — it follows every artifact from delivery through execution, persistence, and early post-exploitation. The goal: document every detection opportunity that existed but wasn't caught.

`Splunk` `Sysmon` `Windows Event Logs` `MITRE T1566 → T1053`

---

### 🧪 Lab 02 — Business Email Compromise (BEC) Investigation
📋 [Full Report →](https://www.notion.so/Business-Email-Compromise-Investigation-300169bd8bbf80d09d62fe6362f561a4)

No malware. No hashes. No lateral file transfers. Just an attacker living inside a trusted identity, manipulating mailbox rules and intercepting communications. This lab focuses on the hardest SOC problem: detecting malicious behavior that looks exactly like legitimate user activity.

`Microsoft Sentinel` `KQL` `Azure AD Audit Logs` `Identity-based detection`

---

<div align="center">

← Back to [Profile](https://github.com/Amadoundiay) &nbsp;·&nbsp; DFIR Reports → [DFIR-Incident-Reports](https://github.com/Amadoundiay/DFIR-Incident-Reports)

</div>
