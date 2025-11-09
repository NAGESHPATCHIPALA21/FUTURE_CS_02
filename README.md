# 🛡️ FUTURE_CS_02 – Security Alert Monitoring & Incident Response

### 👨‍💻 Author: Nagesh Patchipala  
### 🗓️ Date of Report: November 6, 2025  
### 🎓 Internship Domain: Cyber Security – Future Interns  

---

## 📘 Overview
This repository contains my **Task 2 submission** for the **Cyber Security Internship** under **Future Interns**.  
The objective of this task was to simulate a **Security Operations Center (SOC)** environment using a **SIEM tool – Splunk Enterprise**, analyze real-world-style logs, detect incidents, and design an **Incident Response Plan**.  

This project demonstrates the workflow of a **SOC Analyst** — from log ingestion and correlation to threat detection, classification, and response documentation.  

---

## 🧰 Tools & Environment
| Tool | Purpose |
|------|----------|
| **Splunk Enterprise (Free Trial)** | Log analysis, visualization, and correlation |
| **Sample SOC Log Dataset** | Provided test data for simulation |
| **Windows Host (Nagesh-PC)** | Simulated compromised system |
| **Kali Linux (Optional)** | Used for log file preprocessing and analysis |

---

## ⚙️ Methodology
The following structured approach was used for threat detection and response:

1. **Data Ingestion**  
   Imported the provided SOC log dataset into Splunk and verified successful indexing.

2. **Event Analysis**  
   Ran search queries to detect anomalies such as malware, brute-force attempts, and failed logins.

3. **Threat Correlation**  
   Mapped user activity, IPs, and timestamps to connect related events and identify infection patterns.

4. **Visualization**  
   Created dashboards and time-based charts showing frequency and type of detected threats.

5. **Incident Classification**  
   Assigned severity (High/Medium) based on the nature and potential business impact of each incident.

6. **Response Plan Drafting**  
   Documented containment, eradication, and recovery strategies for every major alert.

---

## 🚨 Key Incidents Detected
| Incident | User / IP | Severity | Description |
|-----------|-----------|-----------|--------------|
| **Ransomware Attack** | bob / 172.16.0.3 | 🔴 High | File-encryption activity detected on Nagesh-PC |
| **Rootkit Signature Found** | eve / 10.0.0.5 | 🔴 High | Hidden process indicating unauthorized persistence |
| **Trojan Infection** | david, charlie / 192.172.16.0.3 | 🟠 Medium | Multiple infections spreading through shared resources |
| **Failed Login Attempts** | david / 203.0.113.77 | 🟠 Medium | Possible brute-force credential testing |

---

## 🧩 Incident Response Plan
**Containment :**  
Isolate affected host (Nagesh-PC) and disable compromised accounts.  

**Eradication :**  
Perform full malware scans, remove malicious files, and reimage the affected system.  

**Recovery :**  
Reset credentials, apply OS and application patches, verify data integrity.  

**Awareness :**  
Conduct user awareness sessions about phishing and secure password practices.  

---

## 🧠 Root Cause Analysis
Initial compromise likely resulted from a **phishing email** or **weak/reused credentials**.  
Attackers leveraged these weaknesses to install malware and gain unauthorized access to multiple accounts.  
A full forensic investigation should be performed to confirm the initial infection vector and assess data exposure.

