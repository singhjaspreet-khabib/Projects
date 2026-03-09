# DHCP Failover Lab on Windows Server 2025

## 📌 Project Overview
This project demonstrates a high-availability DHCP infrastructure using Windows Server 2025 failover capabilities in a VMware lab environment.

## 🏗️ Architecture
- **Primary DHCP Server:** DHCP-Primary (10.10.10.20)
- **Secondary DHCP Server:** DHCP-Secondary (10.10.10.30)
- **Network:** Host-only (VMnet19)
- **Domain:** dhcp-lab.local
- **DHCP Scope:** 10.10.10.100 - 10.10.10.200

## ⚙️ Failover Configuration
- **Mode:** Load Balance (50/50)
- **MCLT:** 1 hour
- **Auto State Transition:** Enabled (60 minutes)

## ✅ Test Results
| Test Scenario | Expected Result | Actual Result | Status |
|--------------|----------------|---------------|--------|
| Normal DHCP Request | Client gets IP from pool | Client received 10.10.10.155 | ✅ PASS |
| Primary Server Failure | Secondary continues serving | Client received IP from secondary | ✅ PASS |
| Recovery | Replication successful | Both servers synchronized | ✅ PASS |

## 📸 Screenshots
Under Screenshot folder

## 🔧 Technologies Used
- Windows Server 2025
- Windows 11 Client
- VMware Workstation
- Active Directory Domain Services
- DHCP Failover

## 📝 What I Learned
- DHCP failover configuration
- Importance of MCLT in lease management
- Load balancing concepts for network services
- High availability implementation

## 🔗 Connect With Me
https://www.linkedin.com/in/jaspreet-singh-a-/
