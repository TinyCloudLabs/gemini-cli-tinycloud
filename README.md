# TinyCloud for Gemini CLI

TinyCloud keeps your personal records, like weight, workouts, goals and todos, in your own storage. This Gemini CLI extension tells Gemini CLI how to set up and use TinyCloud through the TinyCloud CLI.

## Install

```sh
gemini extensions install https://github.com/TinyCloudLabs/gemini-cli-tinycloud
```

Start Gemini CLI and ask:

- "Set up TinyCloud for me."
- "Log my weight: 80.5 kg today."

Gemini CLI follows <https://agents.tinycloud.xyz/connect>. It installs the pinned TinyCloud CLI and the `tc-apps` skill in a private folder, then shows you an OpenKey link. Open it, approve, and tell Gemini to continue.

## What it adds

- `GEMINI.md`, a few lines for the model: set up through /connect's coding-agent route, use the `tc-apps` skill for your records, never ask you for a password or other secret, and let you approve access on OpenKey.

It adds no MCP server, commands or hooks. The setup itself installs the CLI and the skill; /connect's Undo section removes them.

## Update or remove it

```sh
gemini extensions update tinycloud
gemini extensions uninstall tinycloud
```

Your records stay in your TinyCloud.

## Gemini CLI docs this follows

- [Extensions](https://geminicli.com/docs/extensions/)
- [Extension reference (`gemini-extension.json`)](https://geminicli.com/docs/extensions/reference/)
- [Release extensions (gallery listing)](https://geminicli.com/docs/extensions/releasing/)
- [MCP servers (`httpUrl`, OAuth discovery, `/mcp auth`)](https://geminicli.com/docs/tools/mcp-server/)

## License

[MIT](LICENSE)
