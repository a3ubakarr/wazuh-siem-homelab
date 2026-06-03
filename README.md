# 🔐 Wazuh SIEM Homelab Project

## 📌 Project Overview
Built a complete Security Operations Center (SOC) lab using 
Wazuh — open-source SIEM/XDR platform — to monitor, detect, 
and respond to real-time security threats across multiple endpoints.

## 🏗️ Architecture
| Machine | Role | OS |
|---------|------|----|
| Ubuntu Server | Wazuh Manager + Indexer + Dashboard | Ubuntu 26.04 |
| Kali Linux | Attacker + Monitored Endpoint | Kali 2026.1 |
| Windows 10 | Victim + Monitored Endpoint | Windows 10 Pro |

## ✅ What I Implemented
- Deployed Wazuh all-in-one stack on Ubuntu Server
- Connected Kali Linux agent (v4.9.0)
- Connected Windows 10 agent (v4.9.0)
- Simulated SSH Brute Force attack using Hydra
- Simulated Port Scanning using Nmap
- Detected and analyzed 192+ alerts in real-time
- Mapped attacks to MITRE ATT&CK framework

## 🎯 Attacks Simulated & Detected
| Attack | Tool Used | Wazuh Detection |
|--------|-----------|-----------------|
| SSH Brute Force | Hydra | ✅ Rule 5712 |
| Port Scanning | Nmap | ✅ Detected |
| Password Guessing | Hydra | ✅ MITRE T1110 |

## 📊 Key Results
- **192+ Authentication Failures** detected
- **MITRE ATT&CK** techniques mapped:
  - T1110 — Brute Force
  - T1110.001 — Password Guessing
  - T1046 — Network Service Scanning
- **3 Endpoints** monitored simultaneously
- **File Integrity Monitoring** active on all agents

## 🛠️ Tech Stack
- **SIEM:** Wazuh v4.9.0
- **Server OS:** Ubuntu Server 26.04
- **Attacker:** Kali Linux 2026.1
- **Endpoint:** Windows 10 Pro
- **Virtualization:** VirtualBox
- **Attack Tools:** Hydra, Nmap


## 🎓 Skills Demonstrated
- SIEM deployment and configuration
- Endpoint Detection & Response (EDR)
- Threat hunting and log analysis
- Attack simulation (Red Team basics)
- MITRE ATT&CK framework mapping
- Linux server administration
- Network configuration (VirtualBox Bridged)

## 📚 References
- [Wazuh Official Documentation](https://documentation.wazuh.com)
- [MITRE ATT&CK Framework](https://attack.mitre.org)
