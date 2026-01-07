# Lab Architecture

This lab consists of three VMs monitored by a central Wazuh SIEM.

## Components
- Wazuh Server (Ubuntu): SIEM Manager, Indexer, Dashboard
- Linux Endpoint (Ubuntu Agent)
- Windows 10 Endpoint (Windows Agent)

## Communication
All agents forward logs securely to the Wazuh server.
