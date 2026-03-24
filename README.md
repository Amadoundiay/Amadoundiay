<div align="center">

```
╔══════════════════════════════════════════════════════════════════════════╗
║                                                                          ║
║        AHMADOU N'DIAYE  ·  DFIR  ·  BLUE TEAM  ·  DETECTION ENG        ║
║                                                                          ║
╚══════════════════════════════════════════════════════════════════════════╝
```

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0072b1?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ahmadoundiaye)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@ndiayeahmadou911)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/p/ahmadoundiaye)

</div>

---

I didn't wait for opportunity. I built the environment, ran the simulations, broke things intentionally, and reverse-engineered why.

No shortcuts. Thousands of hours of deliberate practice — log analysis, failed detections that eventually became good ones, and investigations held to the standard of the analysts I study: DFIR Report, Mandiant, Microsoft DART.

I don't treat security as a certification track. I treat it as a discipline that demands **methodical thinking, forensic precision, and the ability to communicate findings clearly under pressure**.

The work in these repositories reflects that standard. Not aspirationally — demonstrably.

```
  LOG FIRST.       Not assumptions.
  RECONSTRUCT.     Behavior, not just indicators.
  DETECT.          What, when, and how — not just if.
  COMMUNICATE.     Technical precision, executive clarity.
```

---

## Recent Investigations

<table>
<tr>
<td width="50%">

### 🔴 KCD-Web — Pre-Ransomware Staging
**22-day compromise** of a healthcare provider.  
Two threat actors. LSASS credential dump. Java RDP brute forcer disguised as `svchost.exe`. Fake installer deploying a persistent beacon that ran for **55+ hours** before the ransomware command arrived.

Caught during staging. Encryption never executed.

`Splunk` `Sysmon` `Process GUID` `BAM Registry` `VirusTotal`

📄 [Investigation Report →](https://www.notion.so/Investigation-Report-322169bd8bbf8090a2fae1afa6a30962)

</td>
<td width="50%">

### 🔴 Warlock CTF — AD Domain Compromise *(1st Place)*
**Full domain compromise** from a single phishing event.  
KeePass database harvested. WDigest enabled for cleartext credentials. DC and backup server compromised. Shadow copies deleted. `warlock.exe` deployed across multiple systems simultaneously.

`Splunk` `Active Directory` `Event Log Analysis` `Lateral Movement Tracing`

📄 [Investigation Report →](https://www.notion.so/Paging-Dr-Warlock-Reconstruction-of-a-Real-World-Active-Directory-Compromise-Featuring-Stealthy--2ee169bd8bbf80f6b7fcd4c67aa76ad2)

</td>
</tr>
<tr>
<td width="50%">

### 🔴 AMIRMAHDI — Credential Stuffing via Compromised Infrastructure
Threat actor used a compromised server as a **pivot point** to test **277,000+ stolen credentials** against Steam, ExpressVPN, and IPVanish — making criminal activity appear to originate from a trusted network.

`Splunk` `Sysmon` `Authentication Analysis` `Threat Actor Attribution`

📄 [Investigation Report →](https://www.notion.so/INCIDENT-REPORT-ID-1276-313169bd8bbf800295fae5a8b6bd544e)

</td>
<td width="50%">

### 🟠 TA577 — Malware Analysis
End-to-end analysis of a malicious ZIP attributed to **TA577**.  
JavaScript stager → DLL download from 3 attacker-controlled domains → process injection into `SearchProtocolHost.exe` → C2 beaconing every 3 minutes.

`Static Analysis` `Dynamic Analysis` `CAPA` `ANY.RUN` `VirusTotal`

📄 [Lab Report →](./labs/ta577-malware-analysis)

</td>
</tr>
</table>

---

## What I Build

<table>
<tr>
<td width="50%">

### 🚨 DFIR Incident Reports
Professional-grade forensic investigations reconstructing real intrusion scenarios from raw telemetry. Every report includes full attack chain, IOC extraction, 5W1H analysis, and client-facing recommendations.

📂 **[DFIR-Incident-Reports →](https://github.com/Amadoundiay/DFIR-Report)**

</td>
<td width="50%">

### 🔬 SOC Investigation Labs
Structured threat detection exercises covering phishing forensics, BEC analysis, network forensics, and malware analysis — written to analyst standards.

📂 **[SOC-Investigation-Labs →](https://github.com/Amadoundiay/SOC-Labs)**

</td>
</tr>
<tr>
<td width="50%">

### 🛡️ Compromise Assessment Solution *(EY Internship)*
Building a full compromise assessment platform at EY — automated forensic collection via KAPE, detection engineering with Wazuh and custom Sysmon rules, AI-assisted analysis layer, and a React findings dashboard.

`Wazuh` `KAPE` `Sysmon` `Anthropic Claude` `React` `Atomic Red Team`

</td>
<td width="50%">

### 📡 Detection Engineering
Custom Sysmon configurations and Wazuh detection rules built from real attack simulations — covering credential dumping, defense evasion, persistence, and C2 beaconing patterns observed in live investigations.

`Sysmon` `Wazuh` `SIGMA` `MITRE ATT&CK`

</td>
</tr>
</table>

---

## Core Stack

<div align="center">

![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![Microsoft Sentinel](https://img.shields.io/badge/Microsoft_Sentinel-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-3AABE5?style=flat-square&logoColor=white)
![Elastic](https://img.shields.io/badge/Elastic-005571?style=flat-square&logo=elastic&logoColor=white)
![KQL](https://img.shields.io/badge/KQL-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?style=flat-square&logo=windows&logoColor=white)
![KAPE](https://img.shields.io/badge/KAPE-grey?style=flat-square)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white)
![YARA](https://img.shields.io/badge/YARA-FF6B35?style=flat-square)
![Suricata](https://img.shields.io/badge/Suricata-EF3B2D?style=flat-square)
![Active Directory](https://img.shields.io/badge/Active_Directory-0078D4?style=flat-square&logo=microsoft&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-E31B23?style=flat-square)

</div>

---

## Investigation Methodology

Every investigation follows a structured, evidence-first approach:

```
01  SCOPE          →  Identify affected assets, accounts, and time window
02  TRIAGE         →  Authentication anomalies, known malicious indicators
03  TELEMETRY      →  Sysmon process tree, network connections, file events
04  PIVOT          →  Process GUID, LogonID correlation, BAM registry artifacts
05  OSINT          →  VirusTotal, AbuseIPDB, Shodan, threat intelligence
06  RECONSTRUCT    →  Full chronological attack chain with attacker intent
07  REPORT         →  5W1H, IOCs, MITRE mapping, client-facing recommendations
```

> *"The IOC opens the investigation. It does not close it."*

---

## Certifications & Training

| Credential | Status |
|-----------|--------|
| CompTIA Security+ | ✅ Completed |
| EY Cybersecurity Internship | 🔄 Active |
| GCIH (GIAC Certified Incident Handler) | 🎯 Target |

---

---

<div align="center">

**Currently interning at EY Cybersecurity Division**  
Building a production-grade Compromise Assessment Solution

📩 Open to **SOC Analyst** and **DFIR** opportunities  
[Let's connect →](https://www.linkedin.com/in/ahmadoundiaye)

</div>
