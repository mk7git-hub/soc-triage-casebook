# SOC Triage Casebook

Alerts I have triaged on free blue-team platforms, written the way I would hand them to the next shift: what fired, what I checked, what the evidence showed, the verdict, and what I would change in the detection. Each case ends with a **detection-engineering follow-up**, because triage is where good detections come from.

## Method

Every case follows the same five steps ([TEMPLATE.md](TEMPLATE.md)):

1. **Frame:** what the alert claims, the asset and user, why it matters.
2. **Hypotheses:** the malicious and the benign explanation, written before looking at evidence.
3. **Evidence:** the specific queries and artifacts that confirm or refute each hypothesis.
4. **Verdict:** true positive, benign true positive, or false positive, with confidence and the MITRE ATT&CK technique.
5. **Follow-up:** containment steps for a TP, tuning for an FP, and a detection or playbook improvement either way.

Playbooks I use for common alert types are in [`playbooks/`](playbooks).

## Case index

| # | Date | Platform | Alert type | ATT&CK | Verdict | Time to verdict | Follow-up |
| --- | --- | --- | --- | --- | --- | --- | --- |
| | | | | | | | |

## Scorecard

| Metric | Value |
| --- | --- |
| Cases triaged | 0 |
| True positives / benign / false positives | 0 / 0 / 0 |
| Median time to verdict | – |
| Detections or tuning proposals written | 0 |

## Ground rules

- **No answers or flags.** Cases document method and reasoning, not challenge answers. Write-ups are published only for content the platform allows (retired investigations, or platforms that permit write-ups), and never for active graded content.
- **No real customer data.** All data comes from the training platforms' simulated environments.
- **Honest verdicts.** Where I got a case wrong, the case says so and what I learned.

## Platforms

| Platform | Free tier (Nov 2026) | Used for |
| --- | --- | --- |
| LetsDefend (moving into Hack The Box) | 15 SOC alerts per month on the Basic plan | Alert triage in a simulated SIEM queue |
| Blue Team Labs Online | Free investigations | Investigation of logs, PCAPs and endpoints |

Related work: [detection-as-code-pipeline](https://github.com/mk7git-hub/detection-as-code-pipeline) · [cti-threat-briefs](https://github.com/mk7git-hub/cti-threat-briefs)
