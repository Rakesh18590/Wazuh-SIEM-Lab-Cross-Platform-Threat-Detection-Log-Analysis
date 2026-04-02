# Wazuh-SIEM-Lab-Cross-Platform-Threat-Detection-Log-Analysis
Built a cross-platform SIEM lab using Wazuh on Ubuntu with a Windows agent, implementing File Integrity Monitoring (FIM) and brute force attack detection for real-time security monitoring
# 🔐 Wazuh SIEM Home Lab

A hands-on home lab built to practice threat detection,
log analysis and incident response using real tools.

## 🖥️ Lab Environment

| Component | Details |
|---|---|
| SIEM | Wazuh (Manager + Dashboard + Indexer) |
| SIEM OS | Ubuntu 22.04 |
| Domain Controller | Windows Server 2022 (Active Directory) |
| AD Client | Windows 11 |
| Attacker Machine | Kali Linux |
| Hypervisor | Oracle VirtualBox |
| Log Enhancement | Sysmon (SwiftOnSecurity config) |
| Host Machine | Laptop 16GB RAM |

## ✅ Completed Scenarios

### 1. Wazuh SIEM Setup
- Installed Wazuh Manager, Indexer and Dashboard on Ubuntu
- Connected Windows Server as Wazuh agent
- Verified log ingestion in Wazuh dashboard

### 2. File Integrity Monitoring (FIM)
- Configured Wazuh FIM on Windows Server agent
- Monitored critical directories for file changes
- Triggered alerts by creating and modifying files
- Verified alerts in Wazuh dashboard

### 3. Brute Force Attack Detection
- Simulated RDP brute force using Hydra from Kali Linux
- Detected via Windows Event ID 4625 (failed logon)
- Wazuh alerted after multiple failed login attempts
- Observed account lockout Event ID 4740
- MITRE Technique: T1110 — Brute Force

## 📸 Screenshots

### Wazuh Installation

<img width="1461" height="922" alt="wazug-installation" src="https://github.com/user-attachments/assets/b87b4cd8-0ad8-41da-88da-d0b5b79ee2bc" />

### Wazuh Dashboard
<img width="1905" height="923" alt="wazuh-dashboard" src="https://github.com/user-attachments/assets/0a03f09e-2ff9-4070-8566-41d25c8d7a05" />


### Wazuh Manager Status
<img width="767" height="523" alt="wazuh-manager- status" src="https://github.com/user-attachments/assets/b80ac6e4-349c-4835-8b6a-b6d3d445cb21" />

### Agent Status
<img width="1082" height="608" alt="wazuh-agent--status" src="https://github.com/user-attachments/assets/71b186c2-7028-44aa-92d8-861f62f9282f" />

### Brute Force Alert in Wazuh
<img width="1414" height="762" alt="brute-force-alert-wazuh" src="https://github.com/user-attachments/assets/17796329-285d-4d27-b04a-6e070070ca96" />

### Brute Force Attack from Kali (Hydra)
<img width="1696" height="846" alt="brute-force-kali-hydra" src="https://github.com/user-attachments/assets/a37cfe56-2ffb-47d2-a3e9-72cd4ee0e82e" />

### FIM Alert
<img width="1419" height="765" alt="fim-alert" src="https://github.com/user-attachments/assets/b3bcb456-a197-4327-9b71-fda14557d45b" />

## 🛠️ Tools Used
Wazuh · Sysmon · Active Directory · Kali Linux · 
Hydra · VirtualBox · Windows Event Viewer

