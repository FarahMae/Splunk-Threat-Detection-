# 🛡 Splunk SIEM: Windows Log Monitoring 
![Status](https://img.shields.io/badge/Status-Completed-brightgreen) ![Platform](https://img.shields.io/badge/Platform-Windows-blue) ![Log](https://img.shields.io/badge/Log-Splunk_Log-yellow)

This project demonstrates how to use Splunk to monitor various Windows Event Logs for security insights.

## ✅ Use Cases
### 1. Brute-force Login Detection
Detects failed login attempts using EventCode 4625 from Security logs.

### 2. Application Crash Detection
Monitors application logs for forcibly terminated services using EventCode 10024.

### 3. System Event Analysis
Note: No significant data was returned from the system logs during this session, but the query and configuration are included for completeness.
Indexes system logs to monitor general Windows behavior like service startups and shutdowns.

## 📁 Included Files
- `queries/` - SPL queries for each use case
- `report.pdf` - Full documentation of the project
- `screenshots/` - Dashboards and search result visuals

## 🧰 Tools Used
- Splunk Enterprise (Free)
- Windows 10 Event Logs: Security, Application, System
