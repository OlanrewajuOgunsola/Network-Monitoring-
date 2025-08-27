# Splunk Alert Project: Detecting Failed Logins on Windows Server

## Project Overview
This project demonstrates how to configure and trigger a **security alert in Splunk Enterprise** using log data collected from a Windows Server via the **Splunk Universal Forwarder**.  

The alert specifically identifies **multiple failed login attempts (Event ID 4625)**, which may indicate brute-force attacks or unauthorized access attempts.

---

## Architecture & Setup
- **Splunk Universal Forwarder** installed on the Windows Server  
- **Splunk Enterprise** running on the Host PC  
- Forwarder configured to send **Windows Security Event Logs** to Splunk  
- Data indexed under `main` with sourcetype: `WinEventLog:Security`  

**Architecture Diagram (High-Level):**
