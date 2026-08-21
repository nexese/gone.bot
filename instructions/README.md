# GoneBot operating instructions

GoneBot is a set of ordered instructions for an agent harness helping a user make and track the strongest available exposure-reduction request: deletion; persistent suppression, opt-out, or block; then a security freeze or release restriction. Read this index first, then load only the steps needed for the current task.

## Ordered workflow

1. [`01-scope-and-safety.md`](01-scope-and-safety.md) — establish authority, boundaries, and stop conditions.
2. [`02-profile-and-state.md`](02-profile-and-state.md) — identify the minimum required information and choose a local progress file.
3. [`03-broker-selection.md`](03-broker-selection.md) — choose reviewed broker profiles and check harness capabilities.
4. [`04-request-preparation.md`](04-request-preparation.md) — prepare a minimized request from a reviewed template.
5. [`05-approval-and-execution.md`](05-approval-and-execution.md) — preview and approve each browser or email action.
6. [`06-monitoring-and-maintenance.md`](06-monitoring-and-maintenance.md) — reconcile replies, follow up, recheck, pause, export, or remove local progress.

## Source material

- [`../jurisdictions/README.md`](../jurisdictions/README.md) is the short route and wording guide for users outside California or brokers whose choices vary by residence.
- [`../brokers/README.md`](../brokers/README.md) contains broker profiles and their evidence limits.
- [`../templates/README.md`](../templates/README.md) contains request and follow-up text.
- [`../state/progress-template.md`](../state/progress-template.md) defines the flat-file progress format.

## System boundary

GoneBot is human-readable Markdown executed by the user's ChatGPT/Codex or Claude Code harness. It has no application backend, daemon, database, account system, project-owned connector, binary, or background process. Browser, email, authentication, and filesystem capabilities belong to the user's harness. Case progress stays in a user-selected local Markdown file outside this repository unless the user explicitly chooses otherwise.

## Non-goals

GoneBot does not provide legal advice, determine eligibility when it is unclear, support requests outside removal or reduced exposure, monitor another person, bypass security controls, guarantee an outcome, or run unattended background work. A freeze restricts access to a report; it does not erase the information in it. GoneBot does not ship software that connects to providers. The current harness performs authorized browsing, email, and filesystem operations.
