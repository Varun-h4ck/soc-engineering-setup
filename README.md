# SOC Automation Project — Engineering Setup Guide

> Complete infrastructure setup manual for building an automated 
> SOC pipeline from scratch using entirely free tools.
> Total Cost: $0.00

---

## What This Project Builds

A fully automated Security Operations Center workflow pipeline that:
- Collects Windows Event Logs in real time using Winlogbeat
- Stores and analyzes logs in Elastic Cloud SIEM
- Detects 8 attack scenarios using custom KQL rules
- Automates alert triage using N8N workflow engine
- Analyzes alerts using Groq AI (Llama 3.3 70B)
- Enriches IP reputation using AbuseIPDB
- Delivers professional alerts to Slack in under 90 seconds

---

## Tech Stack

| Component | Tool | Cost |
|-----------|------|------|
| SIEM | Elastic Cloud (Kibana) | Free trial |
| Log Shipper | Winlogbeat 9.3.3 | Free |
| Automation Engine | N8N Cloud | Free trial |
| AI Analysis | Groq AI — Llama 3.3 70B | Free tier |
| Threat Intelligence | AbuseIPDB API | Free tier |
| Notifications | Slack | Free tier |
| Hypervisor | VirtualBox | Free |
| Victim Machine | Windows 10 VM | Free |
| Attack Machine | Kali Linux | Free |
| **TOTAL** | | **$0.00** |

---

## Architecture

Windows 10 VM (192.168.56.102)
↓ generates Windows Event Logs
Winlogbeat Agent
↓ ships logs to cloud in real time
Elastic Cloud SIEM
↓ detection rule fires alert
N8N Webhook Node
↓ receives alert JSON payload
Groq AI Node (Llama 3.3 70B)
↓ analyzes + maps MITRE ATT&CK
AbuseIPDB Enrichment Node
↓ checks IP reputation
Slack #alerts Channel
↓
SOC Analyst receives alert in under 90 seconds

---

## What The Report Covers

The full PDF report includes 15 sections:

1. Project Overview and Architecture
2. Prerequisites and Hardware Requirements
3. Account Signups for all platforms
4. VirtualBox and VM Setup
5. Windows 10 VM Configuration and Audit Policies
6. Kali Linux VM Setup
7. Winlogbeat Installation and Configuration
8. Elastic Cloud SIEM Setup
9. All 8 Detection Rules with exact KQL queries
10. N8N Automation Workflow — all 4 nodes
11. Groq AI Integration
12. AbuseIPDB Integration
13. Slack Integration
14. End-to-End Testing and Verification
15. Troubleshooting Guide


---

## Related Project

👉 [SOC Workflow Automation — Threat Detection Scenarios](https://github.com/Varun-h4ck/soc-automation-project)

Project 2 covers all 8 detection scenarios with attack simulations,
Kibana detections and Slack alert outputs.

---

*Educational and portfolio purposes only | Total Cost: $0.00*
