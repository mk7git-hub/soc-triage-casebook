# Playbook: reported or detected phishing email

1. **Header check:** SPF, DKIM, DMARC results; `Return-Path` vs `From`; first external `Received` hop.
2. **Content:** sender lookalike domain, urgency, credential or payment request.
3. **URLs and attachments:** expand short links, check reputation, detonate in a sandbox; hash attachments.
4. **Scope:** search the mail gateway for the same sender, subject, URL or hash across all mailboxes.
5. **Interaction:** did anyone click (proxy logs) or open the attachment (EDR process tree)? Any sign-in from a new IP after the click?
6. **Verdict and action:** purge from mailboxes, block sender/URL/hash, reset credentials for anyone who submitted them, revoke sessions.
7. **ATT&CK:** T1566.001 (attachment), T1566.002 (link), T1078 if credentials were used.
