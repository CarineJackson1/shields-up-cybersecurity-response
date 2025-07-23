# 🛡️ Shields Up: Cybersecurity Incident Response Simulation

**Role:** Information Security Analyst  
**Scenario:** Simulated ransomware attack on AIG using CISA alerts and stakeholder communication  
**Skills:** Python, CISA threat analysis, stakeholder response, incident handling

---

## 📚 Project Overview

In this cybersecurity simulation, I responded to a ransomware attack on AIG by analyzing threat intelligence alerts from the Cybersecurity & Infrastructure Security Agency (CISA), in collaboration with the FBI and NSA.

I developed tools to:
- Parse & interpret CISA JSON threat alerts
- Notify internal stakeholders about high-priority threats
- Simulate a decryption recovery of affected files
- Document the incident timeline and response actions

---

## 🧰 Tools & Technologies
- 🐍 Python
- 🗂 JSON + CSV for alert parsing
- 📄 Text templates for stakeholder communication
- 🔐 Simulated decryption tools

---

## 🔍 Key Components

### 1️⃣ `ransomware_alert_analysis.py`  
Parses CISA alert JSON, identifies ransomware IOCs, and outputs a CSV report.

### 2️⃣ `file_decryptor_sim.py`  
Simulates decrypting a small set of compromised files.

### 3️⃣ `stakeholder_emails/`  
Templates for communicating across departments during an incident, including:
- 📨 `alert_email_template.txt`: General awareness message for internal users
- 🚨 [`critical_alert_advisory.txt`](stakeholder_emails/critical_alert_advisory.txt): Urgent advisory sent to the infrastructure owner during a ransomware event

### 4️⃣ `incident_report.md`  
Incident timeline, severity assessment, mitigation, and recovery notes.

---

## 📊 Outcomes

✅ Applied real-world threat intel  
✅ Demonstrated communication under crisis  
✅ Strengthened detection and response workflows  
✅ Delivered clear documentation for stakeholder and technical audiences

---

## ⚙️ Setup

Install dependencies (if required):

```bash
pip install -r requirements.txt

---
shields-up-cybersecurity-response/
│
├── ransomware_alert_analysis.py
├── recovery_tools/
│   └── file_decryptor_sim.py
├── cisa_alerts/
│   └── alert_sample.json
├── stakeholder_emails/
│   ├── alert_email_template.txt
│   └── critical_alert_advisory.txt
├── docs/
│   └── incident_report.md
└── README.md
```
---
<img width="752" height="493" alt="Screenshot of simulated ransomware response" src="https://github.com/user-attachments/assets/80d31f0e-9976-4dc8-ae7e-cf05751c4077" />

---

## 📧 Sample Stakeholder Communication

### 🚨 `critical_alert_advisory.txt`

> This advisory email notifies infrastructure owners of an active ransomware threat, referencing CISA/FBI/NSA alerts and suggesting mitigation steps (e.g., MFA, patching, RDP lockdown).

Preview:
[View full advisory email »](stakeholder_emails/critical_alert_advisory.txt.pdf)
