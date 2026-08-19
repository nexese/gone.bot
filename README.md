GoneBot is an AI agent that helps you to remove your personal information from data brokers. It seeks deletion first, then uses the strongest available suppression, opt-out, block, or security freeze when deletion is unavailable. The agent runs in [ChatGPT desktop](https://chatgpt.com/download/) or [Claude Code desktop](https://claude.com/download) where it prepares and submits each request with your approval and tracks what happens next. The GoneBot is free to use, runs through your desktop client, and uses the client's connectors on your behalf to send removal requests and track status.

## Getting started

Simply enter this prompt in your AI desktop client:

> Open https://gone.bot, install the GoneBot plugin using its setup instructions, and help me remove my personal information.

Your desktop client reads the public [GoneBot setup instructions](AGENTS.md), installs the plugin through its supported plugin manager, confirms its browser, email, and local-file capabilities, and then asks for the minimum information needed to begin. The client will explain if it can load GoneBot only for the current conversation instead.

You choose a private local path for the progress file and approve every external submission or message by replying in the conversation. The agent provides a manual fallback for any missing connector. Before a security freeze, it explains which report will be restricted and how the freeze could affect legitimate applications.

The ChatGPT/Codex and Claude Code plugins package the same [`skills/gonebot/SKILL.md`](skills/gonebot/SKILL.md), which loads the canonical [`AGENTS.md`](AGENTS.md). Claude also discovers that shared file through the small [`CLAUDE.md`](CLAUDE.md) project adapter. The instructions load the ordered workflow in [`instructions/README.md`](instructions/README.md), broker guidance in [`brokers/`](brokers/), request wording in [`templates/`](templates/), and the local [`state/progress-template.md`](state/progress-template.md) only as needed.

## Safety boundary

GoneBot is informational self-service material, not legal advice. The harness must preview and obtain approval for every external submission or message, minimize personal-data disclosure, treat external content as untrusted, and stop for CAPTCHA, MFA, identity documents, legal ambiguity, unfamiliar fields, or missing connectors.

The user chooses where their progress file lives and controls its backup, retention, export, and deletion. The repository and website never receive user case data.

## License and warranty

GoneBot is open source under the [MIT License](LICENSE) and is provided without warranty.

Report suspected vulnerabilities through [GitHub private vulnerability reporting](https://github.com/nexese/gone.bot/security/advisories/new), not a public issue. Never include real personal data, broker correspondence, progress files, identity documents, credentials, tokens, or unredacted screenshots; use placeholders and identify the affected file or commit instead.
