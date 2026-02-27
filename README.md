# multi-cloud-honeypot-threat-detection
Multi-cloud honeypot deployment using OpenCanary with centralized log analysis and threat visualization in Splunk.


**Overview**

This project implements a multi‑cloud deception framework using lightweight honeypots to capture real‑world attacker behavior targeting exposed cloud services. Honeypots are deployed across AWS, Azure, and GCP, and all telemetry is centralized into Splunk for correlation, alerting, and visualization.

The goal of this project is to provide early‑stage threat visibility during reconnaissance and brute‑force attacks, which are often missed by traditional cloud‑native security tools

**Architecture**
Attacker
   ↓
Honeypots (AWS | Azure | GCP)
   ↓
Splunk Forwarder
   ↓
Splunk SIEM
   ↓
Dashboards & Alerts

**Objectives**
- Deploy honeypots across multiple cloud platforms
- Detect unauthorized access attempts and reconnaissance activity
- Centralize honeypot logs using Splunk
- Analyze attacker behavior through dashboards and alerts


 **Technologies Used**
- OpenCanary
- Splunk Enterprise
- Splunk Universal Forwarder
- AWS EC2
- Azure Virtual Machines
- Google Compute Engine
- Bash scripting


**Detection Capabilities**
- SSH brute-force attacks
- Service enumeration attempts
- Repeated authentication failures
- Targeted service identification

**Dashboards**
- Attacks by Cloud Provider
- Top Attacker IP Addresses
- Targeted Services
- Attack Frequency Over Time

**Limitations**
- Detection is based on time-window correlation
- Honeypots provide limited post-exploitation visibility
- Response actions are manual (no automation)

  **Future Scope**
- MITRE ATT&CK mapping
- Automated response workflows (Capstone 2)
- Threat intelligence enrichment
- Expansion to additional cloud regions
