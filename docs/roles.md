# Roles

Three roles. In a small team two may be the same person, but the responsibilities stay separate.

## Incident commander

- Owns the incident until it is resolved or handed over explicitly.
- Decides: severity, mitigation to attempt, who does what, when to escalate.
- Does not type commands into production while commanding. If they must, they hand over command first.
- Keeps the timeline in the incident channel: what was tried, when, result.

## Operator

- Executes mitigations and diagnostics as directed.
- Reports results in the channel with timestamps, not in private messages.
- Captures evidence before any restart: logs, metrics snapshots, `pg_stat_activity`, error samples.

## Communicator

- Publishes status updates on the cadence for the severity, using the templates.
- Answers customer-facing channels with the approved wording; never speculates on cause.
- Records when each update was sent.

## Handover

Command changes only with an explicit message: "Handing command to X. Current state: ... Next step: ...". Silence is not a handover.

## After resolution

The commander opens the postmortem document, fills the timeline from the channel, and schedules the review within 48 hours.
