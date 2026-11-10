# Case NNN: <short alert name>

| Field | Value |
| --- | --- |
| Date | YYYY-MM-DD |
| Platform / alert ID | LetsDefend #… / BTLO "…" (retired) |
| Alert rule | |
| Severity (platform) | |
| Asset / user | |
| Time to verdict | __ min |

## 1. Frame
What does the alert claim happened, on which asset, and why would it matter to the business?

## 2. Hypotheses (written before investigating)
- **Malicious:**
- **Benign:**

## 3. Evidence
| # | Question | Where I looked (query / tool) | Finding | Supports |
| --- | --- | --- | --- | --- |
| 1 | | | | malicious / benign |

Key artifacts: process tree, parent/child, command line, hashes (reputation), network destinations, user context, timing.

## 4. Verdict
- **Verdict:** True positive / Benign true positive / False positive
- **Confidence:** High / Medium / Low, because …
- **ATT&CK:** Txxxx.xxx (name)

## 5. Follow-up
- **Containment (if TP):** isolate host, disable account, block indicator, preserve evidence
- **Escalation note (3 sentences for Tier 2 / IR):**
- **Detection improvement:** rule change, new Sigma rule, or enrichment that would have made this faster or quieter
- **What I would do differently:**
