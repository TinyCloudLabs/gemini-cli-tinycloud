# TinyCloud

TinyCloud keeps the owner's personal records, such as weight, workouts, goals and todos, in their own storage. You reach it through the TinyCloud CLI and its `tc-apps` skill.

- **Setup:** when the owner asks to set up TinyCloud, or asks for something TinyCloud keeps and it isn't set up yet, follow <https://agents.tinycloud.xyz/connect> in this conversation. You have a shell, so take its coding-agent route: it installs the pinned TinyCloud CLI and the `tc-apps` skill into a private folder. Where the guide asks which client you are, take the Codex choice: its skill folder, `~/.agents/skills`, is the one you read. If shell commands aren't allowed here, say so and stop. Don't claim setup is done before a record reads back.
- **Records:** when the owner asks to log, record, track, add, look up, list or sum up something they keep, read `~/.agents/skills/tc-apps/SKILL.md` and follow it, even if they don't mention TinyCloud.
- **Approval:** the owner approves access on OpenKey. When the CLI prints an OpenKey link, show it to the owner exactly as printed, and wait until they approve and tell you to continue. Don't open the link yourself.
- **Secrets:** never ask for a password, private key, API key, access token or any other secret in chat, and never store one. TinyCloud needs none of them.
