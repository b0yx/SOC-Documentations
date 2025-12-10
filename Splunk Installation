# Splunk Installation & Configuration on Ubuntu

[![Linux](https://img.shields.io/badge/Linux-OS-orange?logo=linux)]()
[![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04%20%7C%2020.04-E95420?logo=ubuntu)]()
[![Splunk](https://img.shields.io/badge/Splunk-Enterprise-000000?logo=splunk)]()
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Lab-blue?logo=hackaday)]()
[![SOC](https://img.shields.io/badge/SOC-Blue%20Team-green)]()

This guide provides clear steps to install and configure **Splunk Enterprise** on Ubuntu for security log collection and analysis.  
Designed for **SOC Analysts, Blue Teamers, DFIR practitioners, and cybersecurity students** building their home labs.

---

## 📑 Table of Contents
- [Requirements](#-requirements)
- [Step 1: Download Splunk](#-step-1-download-splunk)
- [Step 2: Enable Splunk as a Service](#️-step-2-enable-splunk-as-a-service)
- [Optional: Change Splunk Web Port](#-optional-change-splunk-web-port)
- [Step 3: Access Splunk Web Interface](#-step-3-access-splunk-web-interface)

---

## 🖥️ Requirements
- Ubuntu **20.04** or **22.04**
- Terminal access
- Splunk Enterprise (.deb package)
- Internet connection for downloading packages

---

## 📥 Step 1: Download Splunk

Download Splunk using:

```bash
wget -O splunk-9.3.0-51ccf43db5bd-linux-2.6-amd64.deb "https://download.splunk.com/products/splunk/releases/9.3.0/linux/splunk-9.3.0-51ccf43db5bd-linux-2.6-amd64.deb"
Install the package:


sudo dpkg -i splunk-9.3.0-51ccf43db5bd-linux-2.6-amd64.deb
⚙️ Step 2: Enable Splunk as a Service
Navigate to Splunk binaries:


cd /opt/splunk/bin
Enable auto-start + accept license:


sudo ./splunk enable boot-start --accept-license
Start Splunk:


sudo ./splunk start
Set your admin username and password.

🔄 Optional: Change Splunk Web Port
If port 8000 is already in use (e.g., Frappe development), change Splunk's port:


sudo /opt/splunk/bin/splunk set web-port 8001
Restart Splunk after changing port:


sudo /opt/splunk/bin/splunk stop
sudo /opt/splunk/bin/splunk start
🌐 Step 3: Access Splunk Web Interface
Open your browser:


http://<ubuntu-ip>:8000
Or if you changed the port:


http://<ubuntu-ip>:8001
Login using your admin credentials.