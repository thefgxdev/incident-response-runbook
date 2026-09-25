# The first fifteen minutes

Run this before anyone proposes a theory.

## 0 to 2 minutes: declare

- [ ] Open the incident channel with a name and the time.
- [ ] Assign commander and operator by name.
- [ ] Set a provisional severity.
- [ ] Post the first message: what is observed, since when, who is affected.

## 2 to 5 minutes: what changed

- [ ] Last deploys, in every service, in the last 24 hours.
- [ ] Configuration or feature-flag changes.
- [ ] Infrastructure events: provider status page, certificate expiry, DNS changes, scheduled jobs that just ran.
- [ ] Traffic: is this a spike, a campaign, an attack?

Nine incidents out of ten are a change. Find it before diagnosing.

## 5 to 10 minutes: stop the bleeding

Choose the fastest reversible mitigation:

- [ ] Roll back the last deploy.
- [ ] Turn off the feature flag.
- [ ] Fail over to the replica or the other region.
- [ ] Rate limit or block the offending source.
- [ ] Put the system in degraded mode (read-only, queue writes, disable optional features).

Before any restart: capture logs, metrics, active queries, error samples.

## 10 to 15 minutes: confirm and communicate

- [ ] Verify with metrics, not with "it seems better": error rate, latency, the business metric (orders per minute).
- [ ] Publish the first status update using the template.
- [ ] Set the next update time.
- [ ] If not mitigated: escalate, widen the team, revisit "what changed".

## Security incidents: additional steps

- [ ] Preserve evidence; do not wipe or rebuild anything yet.
- [ ] Rotate the credential suspected of compromise; revoke sessions if accounts may be affected.
- [ ] Record the time of detection: notification deadlines (LGPD, GDPR) start here.
- [ ] Limit who knows the details until the scope is understood; communicate through the designated person.

## What not to do

- Do not restart "to see if it helps" before capturing evidence.
- Do not deploy a forward fix under pressure when a rollback exists.
- Do not communicate a cause before it is confirmed.
