# Attack Flow Diagram
[Initial Access]
    ↓
AnyDesk (as-pc2)

    ↓
[Execution]
wsync.exe

    ↓
[Credential Access]
LSASS Dump

    ↓
[Lateral Movement]
as.srv.administrator → as-srv

    ↓
[Reconnaissance]
scan.exe

    ↓
[Tool Transfer]
bitsadmin → PowerShell

    ↓
[Exfiltration]
st.exe → exfil_data.zip

    ↓
[Defense Evasion]
Disable Defender

    ↓
[Impact]
updater.exe → Encryption

    ↓
[Ransom Note]
akira_readme.txt

    ↓
[Anti-Forensics]
clean.bat
