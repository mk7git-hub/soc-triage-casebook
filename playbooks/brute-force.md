# Playbook: brute force or password spray

1. **Shape:** one account many passwords (brute force, T1110.001) or many accounts few passwords (spray, T1110.003)?
2. **Source:** IP reputation, ASN (hosting/VPN providers), geography, prior history.
3. **Success:** any successful logon from the same source or the same window (4624, Entra sign-in success)? If yes, treat as compromise.
4. **Protocol:** legacy protocols (EWS, IMAP, ActiveSync) that skip MFA?
5. **Action:** block source, reset and revoke affected accounts, confirm lockout policy and MFA coverage.
6. **Detection follow-up:** aggregation rule by source and distinct accounts; see the spray hunt in cti-threat-briefs.
