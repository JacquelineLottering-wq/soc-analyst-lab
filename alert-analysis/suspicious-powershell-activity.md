# Alert Investigation: Suspicious PowerShell Activity

## 🕵️ Alert Summary
An alert was triggered due to suspicious PowerShell execution on a Windows endpoint, which may indicate malicious script execution or post-exploitation activity.

---

## ⏱ Timeline of Events
- PowerShell process execution detected
- Command-line arguments flagged as suspicious
- Activity originated from a user workstation

---

## 🔍 Investigation Steps
- Reviewed PowerShell execution logs in the SIEM
- Analysed command-line arguments
- Checked parent process and execution context
- Correlated activity with user behaviour and login events

---

## 🧠 Analysis & Findings
The PowerShell activity used encoded or obfuscated commands commonly associated with malicious behaviour.

No evidence of lateral movement or data exfiltration was observed.

---

## ⚠️ Severity Assessment
**Severity:** Medium–High  
**Reason:** Suspicious script execution with potential malicious intent.

---

## ✅ Conclusion
This activity warrants further monitoring and endpoint inspection.

Recommended actions include:
- Isolating the endpoint if activity persists
- Running endpoint malware scans
- Restricting PowerShell execution policies
- Reviewing user privileges

---

## 📌 Analyst Notes
PowerShell abuse is a common technique used by attackers. Early detection and investigation are critical to prevent escalation.
