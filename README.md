# Sambl Agent Plugins

This repository is the Sambl custom marketplace for Codex, Claude Desktop,
and Claude Code. In the CLI commands, `sambl@sambl` means the **Sambl** plugin
from the **Sambl** marketplace.

Use Sambl with your Sambl UI Kit in Figma. The `sambl` skill connects kit
knowledge, color calculations and optional preparation to your design task.
Use `sambl-style-adaptation` to adapt the kit to screenshots or a named product
style. Your agent uses its Figma tools to inspect and edit the file; the
available connection determines which actions it can perform.

## Install in Codex

### Codex desktop app

1. Open **Codex** in the ChatGPT desktop app and select **Plugins**.
2. Choose **Add → Add a marketplace**.
3. In **Source**, enter either `sambl-ai/agent-plugins` or
   `https://github.com/sambl-ai/agent-plugins.git`, then select
   **Add marketplace**. Leave **Git ref** and **Sparse paths** empty.
4. Choose **Sambl** in the marketplace picker, open the **Sambl** plugin,
   and select **Install plugin**.

[Codex desktop marketplace documentation](https://developers.openai.com/plugins/build/plugins#build-your-own-curated-plugin-list)

### Codex CLI

In your terminal, add the GitHub marketplace and install Sambl from it.

```sh
codex plugin marketplace add https://github.com/sambl-ai/agent-plugins.git
codex plugin add sambl@sambl
```

The first command also accepts `sambl-ai/agent-plugins` in place of the Git URL.
Run `codex plugin marketplace upgrade sambl` to refresh this GitHub source.
[Codex CLI marketplace documentation](https://developers.openai.com/plugins/build/plugins#add-a-marketplace-from-the-cli)

## Install in Claude Desktop

1. In Claude Desktop, open **Customize → Plugins**. In Cowork, open the
   **Cowork** tab first.
2. Choose **Add → Add marketplace → Add from a repository**.
3. Enter either `sambl-ai/agent-plugins` or
   `https://github.com/sambl-ai/agent-plugins`, then select **Sync**.
4. In **Discover**, open the **Sambl** plugin from the **Sambl** marketplace
   and select **Add**.

[Claude desktop marketplace documentation](https://support.claude.com/en/articles/13837440-use-plugins-in-claude#add-or-remove-plugin-marketplaces)

## Install in Claude Code

In your terminal, add the GitHub marketplace and install Sambl from it.
You can use `sambl-ai/agent-plugins` in place of the Git URL in either
marketplace add command below.

```sh
claude plugin marketplace add https://github.com/sambl-ai/agent-plugins.git
claude plugin install sambl@sambl
```

You can also run the following commands from a Claude Code session.

```text
/plugin marketplace add https://github.com/sambl-ai/agent-plugins.git
/plugin install sambl@sambl
/reload-plugins
```

If you installed from the terminal while a session was open, run
`/reload-plugins` in that session. To update manually, run
`claude plugin marketplace update sambl` and then `claude plugin update sambl@sambl`.
[Claude Code plugin documentation](https://code.claude.com/docs/en/discover-plugins)

## Connect and get started

Sign in to Sambl in your browser to connect its MCP server. In the desktop
app, follow the connection prompt for Sambl. In Codex CLI, run
`codex mcp login sambl`. In Claude Code, open `/mcp` and select Sambl.

Connect Figma in your client for tasks that use a Figma file. To edit a kit,
use a copy you have permission to edit.

Try asking **“What can I configure in my Sambl UI Kit?”** Then share a link to
your kit when you want to work on a specific file.

[Sambl](https://sambl.ai/) · [Support](mailto:hi@sambl.ai) ·
[Privacy policy](https://sambl.ai/policy) · [Terms](https://sambl.ai/terms)
