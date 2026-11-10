# Playbook: suspicious PowerShell or command line

1. **Decode:** base64 `-enc` payloads; note download cradles (`IEX`, `DownloadString`, `Invoke-WebRequest`), AMSI bypass strings.
2. **Process tree:** what launched it? Office, browser or `wmiprvse.exe` parents are high risk; an admin's interactive shell is lower.
3. **Network:** destinations contacted in the next minutes; reputation and age of domains.
4. **Persistence:** new scheduled tasks, Run keys, services, WMI subscriptions after the event.
5. **User context:** is this user an admin who runs scripts? Is the time normal for them?
6. **Verdict and action:** isolate if it executed remote code; collect the script block log (4104) as evidence.
7. **ATT&CK:** T1059.001, T1027 (obfuscation), T1105 (ingress tool transfer).
