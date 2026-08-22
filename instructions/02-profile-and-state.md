# 2. Profile and local progress

## Collect only what is needed

Start with non-sensitive facts: jurisdiction and whether the user is acting for themself. Record the user's stated country, state, or region; do not infer it from nationality, language, a broker's location, or an IP address. Use the strongest available exposure-reduction goal and the reviewed, location-appropriate broker set; do not ask the user to select a broker or preferred channel at setup. Load [`../jurisdictions/README.md`](../jurisdictions/README.md) when the user is outside California or the broker's choices vary by residence. Determine required personal fields only from the selected broker profile and current official restriction page.

Sensitive values should remain in the user's chosen local environment. When possible, have the user enter them directly into a browser form or email draft rather than repeating them in conversation.

## Choose one progress file

Propose `~/Documents/gonebot-progress.md` in the user's private Documents directory. Ask them to accept that default or provide another private local Markdown path. Initialize it from [`../state/progress-template.md`](../state/progress-template.md) only after they accept or override the proposed path.

The progress file is the sole GoneBot state. Keep it readable and append factual events. Store minimum identifiers, dates, status, destination, and evidence references—not passwords, tokens, full identity documents, or copied mailbox contents.

Before writing, show the chosen path and what will be recorded. Never silently place the file in the repository, a plugin cache, or a temporary directory. Respect the user's request to pause, export, relocate, redact, or delete it.
