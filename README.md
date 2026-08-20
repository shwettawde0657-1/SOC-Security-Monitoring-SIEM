# SOC Security Monitoring & SIEM

A Security Operations Center (SOC) monitoring and detection project built using Elastic Cloud, Kibana, Elastic Agent and Windows Event Logs.

The project focuses on monitoring Windows authentication activity, detecting suspicious login behavior and investigating security alerts through a SIEM environment.

---

## Project Objective

The objective of this project is to simulate a real-world SOC monitoring environment where security events are collected, analyzed and converted into actionable alerts.

The system monitors Windows authentication events and detects suspicious patterns such as:

- Failed login attempts
- Brute-force login activity
- Failed login followed by successful login
- Suspicious source IP activity

---

## Technologies Used

| Technology | Purpose |
|---|---|
| Elastic Cloud | Cloud-based SIEM environment |
| Kibana | Security monitoring and visualization |
| Elasticsearch | Log storage and search |
| Elastic Agent | Log collection |
| Windows Event Logs | Security event source |
| KQL | Security event queries |
| SIEM Detection Rules | Threat detection and alerting |

---

## Architecture

```text
Windows Machine
      │
      │ Windows Event Logs
      ▼
Elastic Agent
      │
      ▼
Elasticsearch
      │
      ▼
Kibana SIEM
      │
      ├── Discover
      │
      ├── Security Dashboard
      │
      ├── Detection Rules
      │
      └── Alerts
             │
             ▼
       SOC Investigation
