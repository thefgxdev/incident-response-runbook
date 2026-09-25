# Communication templates

Say what you know, when you know it. Never speculate on cause in public.

## Status page: investigating

> **Investigating** · HH:MM UTC
> We are investigating reports of [symptom, in user terms] affecting [who]. [Workaround if any.] Next update by HH:MM.

## Status page: identified

> **Identified** · HH:MM UTC
> We have identified the cause of [symptom] and are applying a fix. [What still works.] Next update by HH:MM.

## Status page: monitoring

> **Monitoring** · HH:MM UTC
> A fix has been applied and [symptom] should be resolved. We are monitoring to confirm. If you still see the issue, [what to do].

## Status page: resolved

> **Resolved** · HH:MM UTC
> The issue affecting [who] between HH:MM and HH:MM UTC has been resolved. We will publish a summary of the cause and the actions we are taking within [N] days.

## Customer email (SEV1, after resolution)

Subject: What happened on [date] and what we are doing about it

Between HH:MM and HH:MM on [date], [what users experienced]. [Whether data was affected, clearly.] The cause was [one sentence, in plain words]. We have [immediate fix] and will [structural fix] by [date]. We are sorry for the disruption. [Contact for questions.]

## Internal channel: update format

```
[HH:MM] STATUS: investigating | identified | monitoring | resolved
Impact: who, how much
Tried: what, result
Next: what, who, by when
```

## Rules

- Updates on the cadence for the severity, even if nothing changed: "still investigating, next update at HH:MM".
- One voice: the communicator, using the commander's facts.
- Time in one time zone, stated.
- After resolution, the public summary is written from the postmortem, not before it.
