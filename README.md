# AI-Enhanced Cyber Defense Lab

A simulated **Security Operations Center (SOC)** environment combining:

- **SIEM-based deterministic detection**
- **Adversary emulation**
- **Machine learning anomaly detection**

The lab demonstrates how modern cyber defense integrates **traditional rule-based monitoring with AI behavioral analytics**.

---

# Architecture Overview

The environment consists of three core nodes:

| Node | OS | Role |
|-----|-----|-----|
| Kali Linux | Linux | Attacker – adversary emulation |
| Metasploitable2 | Linux | Victim – vulnerable infrastructure |
| Ubuntu Server | Linux | SOC – Wazuh SIEM + AI analytics |

**Network Topology**

- VMware **Host-Only Network**
- Subnet: `192.168.56.0/24`
- Fully isolated lab environment for safe attack simulation

---

# Key Technologies

| Category | Tools |
|--------|--------|
| Virtualization | VMware Workstation |
| SIEM | Wazuh |
| Programming | Python |
| ML Libraries | Scikit-learn, Pandas |
| Recon | Nmap |
| Brute Force | Hydra |
| Web Scanning | Nikto |
| Exploitation | Metasploit |

---

# Detection Approach

This project combines **deterministic detection** with **probabilistic machine learning techniques**.

---

## Deterministic Detection (SIEM Rules)

**Wazuh SIEM rules detect:**

- SSH brute force attempts
- Web application attacks
- Reconnaissance scans
- Suspicious authentication activity

Rule-based detection provides **fast and explainable alerts** for known attack patterns.

---

## Probabilistic Detection (Machine Learning)

A **Python-based ML pipeline** analyzes authentication logs using:

- **Isolation Forest**
- **Feature engineering**
- **Anomaly scoring**

This enables detection of **unusual login behavior** that traditional rules may miss.

---

# Repository Structure

docs/ → architecture diagrams and setup guides
src/ → Python ML detection pipeline
config/ → SIEM and syslog configurations
attacks/ → adversary emulation commands
datasets/ → exported logs for analysis
reports/ → incident response documentation
screenshots/ → SIEM dashboards and ML results


---

# Project Goals

This lab demonstrates practical capability in:

- SOC architecture design
- SIEM deployment
- log pipeline engineering
- adversary simulation
- machine learning security analytics
- incident response documentation

---

# Author

Varenya Sawant  
Cybersecurity | Detection Engineering | AI Security
