# osint-learning-journey

# 🛡️ Personal OSINT & Security Auditing with Kali Linux

An educational summary and documentation of performing Open Source Intelligence (OSINT) and credential leak checks on personal assets using **Kali Linux**.

---

## 📌 Overview
This repository documents practical commands and tools used to evaluate personal digital footprint (Phone Number & Email address) for security awareness and data leak prevention.

---

## 🔧 Tools & Workflow

### 1. Phone OSINT (`PhoneInfoga`)
Used to analyze static phone number data, international carrier information, and public search indexings.

#### **Setup & Installation**
```bash
# Step 1: Download the installation script
curl -sSL [https://raw.githubusercontent.com/sundowndev/phoneinfoga/master/support/scripts/install](https://raw.githubusercontent.com/sundowndev/phoneinfoga/master/support/scripts/install) -o install.sh

# Step 2: Execute installation
bash install.sh

# Step 3: Move executable to system PATH
sudo mv ./phoneinfoga /usr/local/bin/

# Step 4: Verify installation
phoneinfoga version
Execution
Bash
# Terminal Scan
phoneinfoga scan -n +212XXXXXXXXX

# Local Web Interface (GUI)
phoneinfoga serve -p 8080
2. Email & Breach OSINT (Holehe & h8mail)
Used to check registered services across various platforms and scan for known historical data breaches.

Setup & Installation
Bash
# Update system dependencies
sudo apt update && sudo apt install python3 python3-pip git -y

# Install tools bypassing managed environment restrictions
pip3 install holehe h8mail --break-system-packages
Execution
Bash
# Check accounts linked to email
holehe your_email@gmail.com

# Check historical breach data
h8mail -t your_email@gmail.com
⚖️ Legal & Ethical Disclaimer
Scope: All activities documented here were performed strictly on personal data and accounts for educational and self-auditing purposes.

Privacy First: OSINT tools gather publicly available data; they do not grant unauthorized access to private messages or accounts.
