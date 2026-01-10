# File Integrity Monitoring (FIM)

This detection demonstrates Wazuh File Integrity Monitoring (FIM) across both Linux and Windows endpoints,
showcasing the ability to detect unauthorized changes to critical system files and registry keys.

---

## Ubuntu Linux Endpoint

### What was monitored
- `/etc/passwd`
- `/etc/cups/subscriptions.conf`
- Custom test files created under `/etc`

### Events detected
- File modification
- File creation
- Integrity checksum changes

### Evidence
![FIM Events – Ubuntu](fim_ubuntu_events.png)

---

## Windows 10 Endpoint

### What was monitored
- Windows Registry keys under `HKEY_LOCAL_MACHINE`
- Service-related registry paths
- System configuration registry values

### Events detected
- Registry key modification
- Registry value modification
- Integrity checksum changes

### Evidence
![FIM Events – Windows 10](fim_windows10_events.png)
