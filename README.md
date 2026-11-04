# Sambl Agent Plugins

Use Sambl with your Sambl UI Kit in Figma. Ask your agent to configure themes,
platforms, and palettes, adjust semantic colors, or build a Sign In or Dashboard
example with the kit's components and styles.

## Install in Codex

Run these commands in your terminal.

```sh
codex plugin marketplace add sambl-ai/agent-plugins
codex plugin add sambl@sambl
```

You can also install Sambl from the **Plugins** tab in the desktop app after
adding the marketplace with the first command. To refresh the marketplace, run
`codex plugin marketplace upgrade sambl`.
[Codex marketplace documentation](https://developers.openai.com/plugins/build/plugins#add-a-marketplace-from-the-cli)

## Install in Claude Code

Run these commands in your terminal.

```sh
claude plugin marketplace add sambl-ai/agent-plugins
claude plugin install sambl@sambl
```

In an open Claude Code session, run `/reload-plugins` to load Sambl. To update
manually, run `claude plugin marketplace update sambl` and then
`claude plugin update sambl@sambl`.
[Claude Code plugin documentation](https://code.claude.com/docs/en/discover-plugins)

## Connect and get started

Sign in to Sambl in your browser to connect the Sambl MCP server. Open the
sign-in flow with `codex mcp login sambl` in your terminal or `/mcp` in Claude
Code. Connect Figma in your client for tasks that use a Figma file. To edit a
kit, use a copy you have permission to edit.

Try asking **“What can I configure in my Sambl UI Kit?”** Then share a link to
your kit when you want to work on a specific file.

[Sambl](https://sambl.ai/) · [Support](mailto:hi@sambl.ai) ·
[Privacy policy](https://sambl.ai/policy) · [Terms](https://sambl.ai/terms)
