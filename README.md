# 🛡️ Shields Up: Cybersecurity Incident Response Simulation

**Role:** Information Security Analyst
**Scenario:** Simulated ransomware attack on AIG using CISA alerts and stakeholder communication
**Skills:** Python, CISA threat analysis, stakeholder response, incident handling

---

## 📚 Project Overview

In this cybersecurity simulation, I responded to a ransomware attack on AIG by analyzing threat intelligence alerts from the Cybersecurity & Infrastructure Security Agency (CISA), in collaboration with the FBI and NSA.

I developed tools to:

* Parse & interpret CISA JSON threat alerts
* Notify internal stakeholders about high-priority threats
* Simulate a decryption recovery of affected files
* Document the incident timeline and response actions

---

## 🧰 Tools & Technologies

* 🐍 Python
* 🗂 JSON + CSV for alert parsing
* 📄 Text templates for stakeholder communication
* 🔐 Simulated decryption tools

---

## 🔍 Key Components

### 1️⃣ `ransomware_alert_analysis.py`

Parses CISA alert JSON, identifies ransomware IOCs, and outputs a CSV report.

### 2️⃣ `file_decryptor_sim.py`

Simulates decrypting a small set of compromised files.

### 3️⃣ `stakeholder_emails/`

Templates for communicating across departments during an incident, including:

* 📨 `alert_email_template.txt`: General awareness message for internal users
* 🚨 [`critical_alert_advisory.txt`](stakeholder_emails/critical_alert_advisory.txt): Urgent advisory sent to the infrastructure owner during a ransomware event

### 4️⃣ `incident_report.md`

Incident timeline, severity assessment, mitigation, and recovery notes.

---

### 5️⃣ `password_bruteforce.py`

**AIG Shields Up: Cybersecurity Virtual Experience Program on Forage – July 2025**

As part of the simulation, I implemented a Python script to assist in an ethical hacking exercise that involved recovering access to encrypted files without paying a ransom.

**Key Activities:**

* Completed a cybersecurity threat analysis simulation for the Cyber Defense Unit, staying updated on CISA publications
* Researched and understood reported vulnerabilities, showcasing analytical skills in cybersecurity
* Drafted a clear and concise email to guide teams on vulnerability remediation
* Utilized Python skills to write a script for ethical hacking, avoiding ransom payments by bruteforcing decryption keys

**Sample Code:**

```python
import zipfile  

def try_password(zip_file, password):
    try:
        zip_file.extractall(pwd=password.encode('utf-8'))
        return True  
    except:
        return False  

def main():
    print("Starting brute-force...")

    with zipfile.ZipFile('/Users/carinejackson/Downloads/EncryptedFilePack/enc.zip') as zf:
        with open('/Users/carinejackson/Downloads/EncryptedFilePack/rockyou.txt', 'r', errors='ignore') as pw_file:
            for line in pw_file:
                password = line.strip()  

                if try_password(zf, password):
                    print(f"[+] Password found: {password}")
                    return  
                else:
                    print(f"[-] Tried: {password}")

    print("[!] Password not found in the list.")

main()
```

---

## 📊 Outcomes

✅ Applied real-world threat intel
✅ Demonstrated communication under crisis
✅ Strengthened detection and response workflows
✅ Delivered clear documentation for stakeholder and technical audiences
✅ Implemented a Python-based brute-force recovery tool during simulation

---

<img width="752" height="493" alt="Screenshot of simulated ransomware response" src="https://github.com/user-attachments/assets/80d31f0e-9976-4dc8-ae7e-cf05751c4077" />

---

## 📧 Sample Stakeholder Communication

### 🚨 `critical_alert_advisory.txt`

> This advisory email notifies infrastructure owners of an active ransomware threat, referencing CISA/FBI/NSA alerts and suggesting mitigation steps (e.g., MFA, patching, RDP lockdown).

Preview:
[Critical Alert Advisory PDF](https://github.com/CarineJackson1/shields-up-cybersecurity-response/blob/main/stakeholder_emails_critical_alert_advisory.txt.pdf)
