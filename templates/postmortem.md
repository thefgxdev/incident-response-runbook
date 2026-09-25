# Postmortem: [title in the form of what happened]

- **Date of incident:** YYYY-MM-DD · **Severity:** SEV1 | SEV2 · **Duration:** HH:MM to HH:MM (N minutes)
- **Commander:** · **Author:** · **Review meeting:** YYYY-MM-DD

## Summary

Three sentences: what users experienced, what caused it, what we are changing.

## Impact

- Users affected: number or share, and how.
- Business impact: orders, revenue, SLA credits, data.
- Detection: how we found out (alert, customer, internal). Time from start to detection.

## Timeline (one time zone)

| Time | Event |
|---|---|
| HH:MM | First error appears in logs (found later) |
| HH:MM | Alert fires / customer reports |
| HH:MM | Incident declared, commander assigned |
| HH:MM | Mitigation attempted: ... result: ... |
| HH:MM | Mitigated |
| HH:MM | Resolved |

## Root cause and contributing factors

The direct cause in one paragraph. Then the factors that let it happen or made it worse: missing alert, missing test, missing timeout, missing runbook, tribal knowledge. Blameless: the system allowed it.

## What went well

Honestly. Fast detection, a rollback that worked, a runbook that was followed.

## What went badly

Honestly. Slow detection, a restart that destroyed evidence, an update that was late.

## Action items

| Action | Owner | Due | Status |
|---|---|---|---|
| Add alert on ... | name | YYYY-MM-DD | open |
| Add test for ... | name | YYYY-MM-DD | open |
| Write runbook for alert ... | name | YYYY-MM-DD | open |

Every action has a person and a date. Actions without an owner are wishes.

## Lessons for the playbook

What in the shared runbooks or checklists should change because of this incident.
