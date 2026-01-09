# Linux Agent

## Description
This document describes the deployment and enrollment of the Linux (Ubuntu) agent into the Wazuh SIEM environment.

## Environment
- **OS:** Ubuntu Linux
- **Role:** Wazuh Agent
- **Connection:** Secure communication with Wazuh Manager

## Installation & Enrollment
The Wazuh agent was installed using the official Wazuh package repository.  
During installation, the agent was enrolled with the Wazuh Manager using an authentication key generated on the manager.

## Logging & Monitoring
The Linux agent is configured to provide:
- System and authentication logs
- File Integrity Monitoring (FIM)
- Audit-based monitoring for privilege escalation
- User and group account activity

## Validation
Successful enrollment was confirmed by the agent appearing as **Active** in the Wazuh Dashboard.

📸 *See `screenshots/02-Agents-connected.png` for agent connection verification.*
