# Executive Summary

A ransomware incident attributed to an Akira affiliate was investigated within a controlled environment. The attacker leveraged pre-staged access to re-enter the network and execute a multi-stage intrusion.

The attack involved credential theft, lateral movement, data exfiltration, and ransomware deployment. Anti-forensics techniques were used to remove evidence post-execution.

## Impact

- Systems affected: as-pc2, as-srv
- Data exfiltrated prior to encryption
- File encryption completed successfully
- Recovery mechanisms were disabled

## Root Cause

- Reuse of pre-staged remote access (AnyDesk)
- Lack of detection for credential theft and lateral movement

## Key Findings

- PowerShell used for payload delivery
- LSASS memory accessed for credential harvesting
- Administrator account used for lateral movement
- Data staged and compressed before exfiltration
- Ransomware deployed as disguised binary (updater.exe)
- Cleanup script executed to remove artifacts

## Recommendations

- Disable unauthorized remote access tools
- Enable PowerShell logging and monitoring
- Monitor LSASS access attempts
- Detect execution from ProgramData directory
- Implement EDR rules for shadow copy deletion
