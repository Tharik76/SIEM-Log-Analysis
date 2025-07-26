# SIEM-Log-Analysis
SOC Analyst practice project with sample logs and Splunk queries
# 🔐 SIEM Log Analysis

This project contains practice materials for SOC Analyst training, focusing on log analysis, detection, and alert building using real-world examples.

## 📂 Contents

- 📁 Apache access log samples
- 📁 Windows Event Log samples
- 📁 Linux auth & cron logs
- 🔍 Sample Splunk search queries
- ⚠️ Use cases for alert detection (login failure, brute force, privilege escalation)

## 🛠 Tools Used

- Splunk Free
- TryHackMe Labs
- Log Parser
- Sysmon & Event Viewer

## 📈 Sample Use Case

index=windows source="WinEventLog:Security" EventCode=4625
| stats count by Account_Name, host
| where count > 5

yaml
Copy
Edit


📝 This detects multiple failed logins which may indicate brute-force attack.

## 📚 Learning Goals

- Understand different types of logs
- Build correlation rules
- Practice writing detection logic

---

🧠 *Practice. Analyze. Detect. That’s the way to be a real SOC Analyst.* 💪

