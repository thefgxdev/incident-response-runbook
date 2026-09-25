# Severity levels

| Level | Definition | Examples | Response | Update cadence |
|---|---|---|---|---|
| **SEV1** | Core function down or data being lost or exposed, for most users | Checkout down, login down, data leak, corruption in progress | Page on-call immediately, commander assigned in 5 min, all hands as needed | Every 30 min, status page public |
| **SEV2** | Core function degraded or down for a subset; important function down | p99 10× normal, one region down, payments failing for one method | Page on-call, commander in 15 min | Every hour |
| **SEV3** | Important function degraded, workaround exists | Search slow, emails delayed, reports failing | Ticket, handled in business hours next day | Daily until resolved |
| **SEV4** | Cosmetic or internal | Dashboard wrong, log noise | Backlog | None |

## Rules

- When in doubt, declare the higher severity. Downgrading is cheap; discovering an hour later that it was a SEV1 is not.
- Security incidents (suspected breach, leaked credential) are SEV1 until proven otherwise, and follow the additional steps in the security section of the first-fifteen-minutes checklist.
- The commander may change severity; the change is logged in the incident channel with the reason.

## Who is paged

- SEV1 and SEV2: the on-call engineer, then the escalation contact if no acknowledgement in 10 minutes.
- SEV1 additionally: the person responsible for customer communication.
- Security SEV1 additionally: whoever owns legal and data-protection obligations, because notification deadlines start at detection.
