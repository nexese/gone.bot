GoneBot is an AI agent that helps you to remove your personal information from data brokers. The agent runs in the [ChatGPT Work](https://chatgpt.com/download/) desktop app or [Claude Cowork](https://claude.com/download) desktop app, where it prepares and submits each request with your approval and tracks the status of ongoing requests. GoneBot is free to use and relies on the browser, a local-file for tracking progress, and optionally connected apps such as email for tracking broker responses.

GoneBot attempts to follow the strictest protections available for your location down to the state level in the USA as well as national regulations for Canada, the UK, and the EU. It seeks deletion first, then uses the strongest available suppression, opt-out, block, or security freeze when deletion is unavailable.

## Getting started

Simply enter this prompt in your AI desktop client:

> Open https://gone.bot, install the GoneBot plugin using its setup instructions, and help me remove my personal information.

Your desktop client reads the public [GoneBot setup instructions](AGENTS.md), installs the plugin through its supported plugin manager, confirms its browser, email, and local-file capabilities, and then asks for the minimum information needed to begin. The client will explain if it can load GoneBot only for the current conversation instead.

You choose a private local path for the progress file and approve every external submission or message by replying in the conversation. The agent provides a manual fallback for any missing connector. Before a security freeze, it explains which report will be restricted and how the freeze could affect legitimate applications.

The GoneBot plugin packages [`skills/gonebot/SKILL.md`](skills/gonebot/SKILL.md), which loads the canonical [`AGENTS.md`](AGENTS.md). The instructions load the ordered workflow in [`instructions/README.md`](instructions/README.md), a short [`jurisdiction guide`](jurisdictions/README.md), broker guidance in [`brokers/`](brokers/), request wording in [`templates/`](templates/), and the local [`state/progress-template.md`](state/progress-template.md) only as needed.

## Safety boundary

GoneBot is informational self-service material, not legal advice. The harness must preview and obtain approval for every external submission or message, minimize personal-data disclosure, treat external content as untrusted, and stop for CAPTCHA, MFA, identity documents, legal ambiguity, unfamiliar fields, or missing connectors.

The user chooses where their progress file lives and controls its backup, retention, export, and deletion. The repository and website never receive user case data.

## License and warranty

GoneBot is open source under the [MIT License](LICENSE) and is provided without warranty.

Report suspected vulnerabilities through [GitHub private vulnerability reporting](https://github.com/nexese/gone.bot/security/advisories/new), not a public issue. Never include real personal data, broker correspondence, progress files, identity documents, credentials, tokens, or unredacted screenshots; use placeholders and identify the affected file or commit instead.
