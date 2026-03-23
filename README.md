# SOC Automation Lab
<p>
  <img src="https://img.shields.io/badge/Wazuh-SIEM-blue?style=flat&logo=elastic" />
  <img src="https://img.shields.io/badge/Shuffle-SOAR-green?style=flat" />
  <img src="https://img.shields.io/badge/TheHive-Incident_Response-orange?style=flat" />
  <img src="https://img.shields.io/badge/Sysmon-Windows-black?style=flat&logo=windows" />
  <img src="https://img.shields.io/badge/VirusTotal-API-blue?style=flat&logo=virustotal" />
</p>

## Overview
This project presents a hands-on Security Operations Center (SOC) Automation Lab designed to simulate real-world security monitoring, alert enrichment, and incident response workflows.

The lab integrates Wazuh (SIEM), Shuffle (SOAR), and TheHive (incident response platform) to automate detection, analysis, and case creation.

## Architecture Diagram

![SOC Architecture](screenshots/architecture-diagram.png)

This diagram illustrates the end-to-end SOC workflow, including log collection, alert detection, enrichment, and automated incident response using Wazuh, Shuffle, and TheHive.

## Workflow
1. Sysmon generates endpoint logs
2. Wazuh analyzes logs and triggers alerts
3. Alerts are sent to Shuffle via webhook
4. Shuffle extracts indicators (hash/IP)
5. VirusTotal enriches the alert
6. TheHive creates a case automatically
7. Analyst reviews and investigates

## Objectives
- Detect suspicious activity using Wazuh
- Automate alert enrichment using VirusTotal API
- Build automated workflows using Shuffle (SOAR)
- Create incident cases in TheHive
- Simulate SOC analyst investigation process

## Architecture
- Wazuh (SIEM) on Ubuntu
- TheHive (Case Management)
- Shuffle (SOAR automation)
- Windows 10 endpoint with Sysmon

## Detection Example
- Attack: Credential Dumping
- Tool: Mimikatz
- MITRE ATT&CK: T1003

## Tools Used
- Wazuh
- TheHive
- Shuffle
- Sysmon
- VirusTotal API

## Results
- Successful detection of simulated attacks
- Automated case creation
- Real-time alert enrichment
- Reduced manual SOC workload

## Lessons Learned
- SOC automation improves response speed
- SIEM + SOAR integration is powerful
- Open-source tools can build real SOC environments
- SOC automation improves response speed
- SIEM + SOAR integration is powerful
- Open-source tools can build real SOC environments

## Sample Investigation
- [Mimikatz Credential Dumping Investigation](investigations/mimikatz-investigation.md)

## Screenshots

### TheHive Alert Dashboard
![TheHive Alert Dashboard](screenshots/thehive-alert-dashboard.png)

### TheHive Case Details
![TheHive Case Details](screenshots/thehive-case-details.png)

### Wazuh Alert (Credential Dumping Detection)
![Wazuh Alert](screenshots/wazuh-alert.png)

### Shuffle SOAR Workflow
![Shuffle Workflow](screenshots/shuffle-workflow.png)

### Automated Email Alert (SOAR Output)
![Email Alert](screenshots/email-alert.png)

