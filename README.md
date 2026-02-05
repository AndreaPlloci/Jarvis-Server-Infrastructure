# Jarvis Server Infrastructure - AI Ops & Monitoring 🖥️🛡️

This repository documents the private server infrastructure that hosts the Jarvis AI ecosystem. It focuses on system reliability, data sovereignty, and proactive resource management.



## 🏗️ Hardware & OS Architecture
* **Server Node:** Headless Windows Server environment optimized for 24/7 AI orchestration.
* **Resilience:** BIOS-level "Power On" configuration to ensure auto-reboot after power failures.
* **Storage:** Hybrid SQL setup with **MariaDB** and **MySQL** for high-precision auditing and financial data.
* **Backup:** Automated daily ETL tasks for database mirroring and off-site storage on Google Drive.

## 🛡️ Network & Security
* **VPN:** Zero-trust mesh networking via **Tailscale**, ensuring no open ports to the public internet.
* **DNS Filtering:** **AdGuard Home** integration for network-wide telemetry blocking and DNS sinkholing.
* **Privacy:** All AI agents interact with local databases, maintaining total data sovereignty.

## 📈 Proactive Monitoring (Health Hub)
The system monitors its own vitals every 30 minutes to ensure peak performance for RAG operations:
* **Automation:** n8n workflows integrated with local **PowerShell** scripts.
* **Telemetry:** Captures CPU usage, RAM availability, and Disk health via WMI classes.
* **Alerting:** Real-time Telegram notifications for system anomalies and SQL logging for historical trend analysis.

## 📂 Repository Structure
* `scripts/`: PowerShell (.ps1) scripts for system interrogation.
* `n8n-workflows/`: JSON exports for the Health Monitor (Auto & Manual).

---
*Designed for maximum uptime and secure industrial-grade automation.*
