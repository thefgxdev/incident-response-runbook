# Runbook: [alert name]

Every alert that can page a human has one of these. If an alert has no runbook, it is noise.

- **Alert:** exact name and query.
- **Severity when it fires:** SEV1 | SEV2 | SEV3.
- **Owner:** team and escalation contact.

## What it means

One paragraph: what the metric measures, what a firing alert usually indicates, and what it can be confused with.

## First checks (5 minutes)

1. Dashboard link: what to look at first.
2. Recent deploys and changes for the affected service.
3. The one query or command that confirms or rules out the usual cause.

## Mitigation

Ordered from fastest and safest:

1. ...
2. ...

Each step: the exact command or click, the expected effect, how to verify, how to undo.

## Escalation

When to escalate, to whom, and what to include in the message.

## Known causes and fixes

| Symptom | Cause | Fix |
|---|---|---|
| | | |

## Last reviewed

YYYY-MM-DD by name. Review after every incident that used this runbook.
