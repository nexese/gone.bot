# 2. Profile and local progress

## Collect only what is needed

Start with non-sensitive facts: desired outcome, jurisdiction, broker, preferred channel, and whether the user is acting for themself. Determine required personal fields only from the selected broker profile and current official restriction page.

Sensitive values should remain in the user's chosen local environment. When possible, have the user enter them directly into a browser form or email draft rather than repeating them in conversation.

## Choose one progress file

Ask the user where to keep a local Markdown progress file. If they have no preference, suggest `gonebot-progress.md` in a private directory they control. Initialize it from [`../state/progress-template.md`](../state/progress-template.md).

The progress file is the sole GoneBot state. Keep it readable and append factual events. Store minimum identifiers, dates, status, destination, and evidence references—not passwords, tokens, full identity documents, or copied mailbox contents.

Before writing, show the chosen path and what will be recorded. Never silently place the file in the repository, a plugin cache, or a temporary directory. Respect the user's request to pause, export, relocate, redact, or delete it.
