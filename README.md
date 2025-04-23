# 🛡 Splunk SIEM: Windows Threat Detection Project

This project uses Splunk to detect brute-force login attempts on a Windows machine by monitoring Event Logs in real time.

## 🎯 Use Case: Brute-force Detection
Detect repeated failed logins (EventCode 4625) using SPL:


index=main OR index=default sourcetype=WinEventLog:Security EventCode=4625
| stats count by Account_Name, Workstation_Name
| where count > 5
```

## 🧰 Tools Used
- Splunk Enterprise (Free Trial)
- Windows 10
- Local Event Logs: Security, System

## 📁 Folder Structure
- `queries/` - SPL detection queries
- `screenshots/` - Dashboard screenshots
- `report.pdf` - Full documentation of the use case

## ✅ Result
Splunk successfully detected 10 failed login attempts for user `FARAWAY$`, displayed in the dashboard titled `Windows Threat Monitoring`.
