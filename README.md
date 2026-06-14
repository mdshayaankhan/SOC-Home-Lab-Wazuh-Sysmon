# SOC Home Lab using Wazuh and Sysmon for Real-Time Threat Detection

## Overview

This project demonstrates the implementation of a Security Operations Center (SOC) Home Lab using Wazuh SIEM and Microsoft Sysmon for real-time endpoint monitoring, log analysis, threat detection, and security event investigation.

The lab simulates a real-world SOC environment where security events generated on a Windows endpoint are collected, analyzed, and visualized through Wazuh. The project showcases practical experience in SIEM administration, threat hunting, endpoint monitoring, MITRE ATT&CK mapping, and incident investigation.

---

## Objectives

* Build a functional SOC Home Lab environment.
* Monitor endpoint activities in real time.
* Centralize security log collection and analysis.
* Detect suspicious activities using SIEM rules.
* Perform threat hunting and alert investigation.
* Map detected activities to the MITRE ATT&CK framework.
* Demonstrate practical SOC Analyst skills.

---

## Architecture

```text
Windows 11 Endpoint
       │
       │ Sysmon Events
       ▼
   Wazuh Agent
       │
       │ Log Forwarding
       ▼
Ubuntu Server
(Wazuh Manager + Indexer + Dashboard)
       │
       ▼
Threat Hunting & Alert Analysis
```

---

## Technologies Used

* Ubuntu Server 24.04
* Wazuh SIEM
* Wazuh Manager
* Wazuh Dashboard
* Wazuh Agent
* Microsoft Sysmon
* Windows 11
* MITRE ATT&CK Framework

---

## Features Implemented

### Endpoint Monitoring

* Connected Windows 11 endpoint to Wazuh using Wazuh Agent.
* Continuous collection of security events.

### Sysmon Integration

* Installed and configured Microsoft Sysmon.
* Captured process creation and system activity events.
* Enhanced endpoint visibility.

### Threat Hunting

* Investigated security events using Wazuh Threat Hunting.
* Filtered and analyzed endpoint telemetry.

### MITRE ATT&CK Mapping

* Detected activities mapped to MITRE ATT&CK techniques.
* Examples:

  * T1059.001 – PowerShell
  * T1059.003 – Windows Command Shell
  * T1087 – Account Discovery
  * T1565.001 – File Modification

### File Integrity Monitoring (FIM)

* Monitored file modifications and integrity changes.
* Generated alerts for file activity.

### Registry Monitoring

* Detected registry key modifications and deletions.
* Generated security alerts for registry events.

### Real-Time Alerting

* Generated alerts for suspicious command execution and system activity.
* Centralized alert visualization through Wazuh Dashboard.

---

## Demonstration Scenarios

### Command Execution Detection

Commands executed:

```cmd
whoami
hostname
ipconfig
net user
```

Detected by:

* Sysmon
* Wazuh SIEM
* MITRE ATT&CK Mapping

---

### PowerShell Monitoring

Commands executed:

```powershell
Get-Process
Get-Service
Get-LocalUser
```

Generated PowerShell-related events and detections.

---

### File Integrity Monitoring

Actions performed:

```powershell
echo "test" > C:\SOC_Test\test.txt
Add-Content C:\SOC_Test\test.txt "modified"
Remove-Item C:\SOC_Test\test.txt
```

Detected by:

* Wazuh File Integrity Monitoring
* Integrity Checksum Change Alerts

---

## Results

Successfully implemented:

* Centralized log collection
* Endpoint monitoring
* Sysmon event collection
* Threat hunting
* MITRE ATT&CK mapping
* File integrity monitoring
* Registry monitoring
* Real-time alert generation

The SOC Home Lab provides hands-on experience with technologies and workflows commonly used by Security Operations Center (SOC) Analysts.

---

## Screenshots

Add screenshots for:

* Architecture Diagram
* Wazuh Dashboard
* Agent Connected
* Sysmon Events
* Threat Hunting
* MITRE ATT&CK Alerts
* File Integrity Monitoring Alerts
* Registry Monitoring Alerts

---

## Skills Demonstrated

* Security Operations Center (SOC)
* SIEM Administration
* Wazuh
* Sysmon
* Threat Hunting
* Log Analysis
* Incident Investigation
* Endpoint Monitoring
* File Integrity Monitoring
* Registry Monitoring
* MITRE ATT&CK
* Windows Security
* Linux Administration

---

## Author

**Md Shayaan Khan**

Computer Science & Engineering Student | Cybersecurity Enthusiast | SOC Analyst Aspirant
