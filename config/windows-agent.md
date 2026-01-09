# Windows Agent

## Description
This document describes the deployment and enrollment of the Windows 10 agent into the Wazuh SIEM environment.

## Environment
- **OS:** Windows 10
- **Role:** Wazuh Agent
- **Connection:** Secure communication with Wazuh Manager

## Installation & Enrollment
The Wazuh agent was installed using the official Windows installer.  
The agent was enrolled with the Wazuh Manager using an authentication key and configured to forward Windows Security events.

## Logging & Monitoring
The Windows agent provides:
- Windows Security Event logs
- File Integrity Monitoring (FIM)
- User and group account management events
- Privilege-related activity via Security logs

## Validation
Successful enrollment was confirmed by the agent status showing **Active** in the Wazuh Dashboard.

📸 *See `screenshots/02-Agents-connected.png` for agent connection verification.*
