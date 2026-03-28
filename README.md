Cisco Interface Utilization Monitoring using Ansible
📌 Overview

This project automates monitoring of Cisco interface utilization across multiple devices using Ansible.

It is designed to help network teams proactively detect high utilization, avoid congestion, and maintain optimal performance.

🚀 Features

* Multi-device monitoring
* Multi-interface support
* Bandwidth utilization calculation (Mbps & %)
* Threshold-based alerting:

  * NORMAL
  * WARNING
  * CRITICAL
* Centralized audit logging
* Email notification
* Zoho Cliq alert integration
* Scalable inventory-based design

🏗️ Architecture

Cisco Devices
     │
     │ (SSH)
     ▼
Ansible Control Node
     │
     ▼
Data Processing Logic
     │
     ├── Audit Logs
     ├── Email Alerts
     └── Zoho Cliq Notifications

## 📂 Project Structure

playbooks/     → Core automation logic  
vars/          → Interface mapping & bandwidth config  
logs/          → Sample outputs & logs  

⚙️ How It Works

1. Connects to Cisco devices via SSH
2. Collects interface statistics
3. Calculates utilization based on configured bandwidth
4. Categorizes utilization (Normal/Warning/Critical)
5. Logs results and sends alerts

📊 Sample Output

Device: DC_SW_WAN_001
Interface: GigabitEthernet0/0
Input Rate: 120 Mbps
Output Rate: 95 Mbps
Utilization: 78%
Status: WARNING

🛠️ Tech Stack

* Ansible
* Cisco IOS
* SSH (CLI-based automation)

⚠️ Note

This repository contains a **simplified version** of a production-grade automation framework.

The full version includes:

* Advanced error handling
* Multi-device orchestration
* Enhanced validation logic
* Enterprise logging mechanisms

👨‍💻 Author

Santosh Kumar Mohapatra
Network Automation Engineer | 11+ Years Experience

