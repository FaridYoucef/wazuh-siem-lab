Privilege Escalation:

Ubuntu Agent (Linux):

Wazuh detected a sequence of high-risk file system changes involving sudo-related files:

Creation and deletion of sudoers temporary files

Modification of /etc/subuid

This behavior is consistent with attempts to modify privilege boundaries using tools such as visudo or manual sudoers manipulation.

MITRE ATT&CK mapping:

T1548.003 – Abuse Elevation Control Mechanism

T1098 – Account Manipulation

Why this matters

Manipulating sudoers and subuid files allows attackers to escalate privileges to root, bypass security controls, and gain persistent administrative access.

Windows 10 Agent:

Wazuh detected a high-severity privilege escalation event when a user was added to the local Administrators group.

This action was captured via Windows Security Event ID 4732, which logs changes to security-enabled local groups.

Key alert details:

Rule ID: 60154

Severity Level: 12 (High)

Description: Administrators Group Changed

MITRE ATT&CK mapping:

T1484 – Domain Policy Modification

Tactic: Privilege Escalation, Defense Evasion

Why this matters

Adding a user to the Administrators group grants full system privileges, enabling attackers to disable defenses, execute privileged commands, and establish persistence.
