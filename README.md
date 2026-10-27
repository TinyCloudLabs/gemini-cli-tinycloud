# TinyCloud for Gemini CLI

TinyCloud keeps your personal records, like weight, workouts, goals and todos, in your own storage. This Gemini CLI extension connects Gemini CLI to TinyCloud's hosted MCP server.

## Install

```sh
gemini extensions install https://github.com/TinyCloudLabs/gemini-cli-tinycloud
```

Start Gemini CLI, then sign in:

```text
/mcp auth tinycloud
```

Your browser opens OpenKey. Sign in and approve. Then ask, for example:

- "What personal apps do I already have in TinyCloud?"
- "Log my weight: 80.5 kg today."

The first time, a TinyCloud tool shows you an OpenKey link for access to your records. Open it, approve, and tell Gemini to continue.

The sign-in needs a web browser on the same computer. It doesn't work over SSH or in a container without one.

## What it adds

- One MCP server, `tinycloud`, at `https://mcp.tinycloud.xyz/mcp`. Gemini CLI finds the server's OAuth settings and registers itself, so there is no key or client ID to enter. It keeps the sign-in in `~/.gemini/mcp-oauth-tokens.json`.
- `GEMINI.md`, a few lines for the model: use the TinyCloud tools for your records, never ask you for a password or other secret, and let you approve access on OpenKey.

It adds no commands, hooks or local programs.

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
