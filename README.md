# Incident Response Runbook

Templates and procedures for the moment something is down: severity levels, roles, the first fifteen minutes, communication, and the postmortem that turns an incident into a system improvement instead of a war story.

By [Felipe Guedes](https://fgxdev.com). Built for small and medium engineering teams that do not have a dedicated SRE function yet.

## Contents

- [`docs/severity.md`](docs/severity.md): four levels, what each one means, who is paged, how fast.
- [`docs/roles.md`](docs/roles.md): incident commander, operator, communicator. Three roles, even if two are the same person.
- [`docs/first-fifteen-minutes.md`](docs/first-fifteen-minutes.md): the checklist that runs before anyone theorises.
- [`docs/communication.md`](docs/communication.md): templates for the status page, customers and the internal channel, by severity.
- [`templates/postmortem.md`](templates/postmortem.md): blameless, with a timeline, contributing factors and owned action items.
- [`templates/runbook.md`](templates/runbook.md): the template for a per-alert runbook, so every alert has a first response written down.

## Principles

1. **Stop the bleeding, then find the cause.** Rollback, failover, kill switch, rate limit. Diagnosis happens on a stable system.
2. **One commander.** Decisions go through one person; everyone else executes or reports.
3. **Say what you know, when you know it.** A status update every 30 minutes, even if it is "still investigating".
4. **Capture evidence before restarting.** Restarts clear symptoms and destroy the trail.
5. **Blameless postmortem, owned actions.** The system allowed the failure; the fix is in the system.

## Em português

Runbook de resposta a incidentes para equipes pequenas e médias: severidades, papéis, os primeiros quinze minutos, comunicação e postmortem sem culpa com ações com dono.

## License

Apache-2.0. Copyright (c) 2026 Felipe Guedes (fgxdev.com). Redistributions must keep the NOTICE file and mark any changes.
