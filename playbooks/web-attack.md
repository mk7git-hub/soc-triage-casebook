# Playbook: web application attack alert (SQLi, XSS, command injection, LFI)

1. **Request:** decode the URL and body; identify the payload class.
2. **Response:** status code and response size; a 200 with an unusually large or error-containing response suggests success.
3. **Follow-on:** more requests from the same IP, new files in the web root, outbound connections from the web server.
4. **Asset:** is the targeted app actually vulnerable (version, WAF in block mode)?
5. **Verdict:** attempt only (blocked or failed) vs successful exploitation.
6. **Action:** block IP, patch or virtual-patch, hunt for webshells if success is possible.
7. **ATT&CK:** T1190, T1505.003 (web shell) if a shell is found.
