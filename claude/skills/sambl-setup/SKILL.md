---
name: sambl-setup
description: Prepare or restore Sambl and Figma access in Claude Desktop, Cowork or Claude Code, recover a provider access denial, or resolve the working Figma file before a Sambl design task. Use when the required connection or target is missing, denied or uncertain.
---

# Prepare Sambl access in Claude

Retain the user's task and answers. Read [the selected connection](references/connection.json)
and [external-agent preparation](../../references/external-agent-setup.md), then
continue the requested product skill when its necessary access is ready.
For installation/MCP health use sambl-check; kit configuration belongs to
sambl-onboarding or the requested specific product skill.

Reuse the exact installed Sambl environment. In Desktop/Cowork, locate this
plugin in Settings → Plugins → Yours and use its Sambl connector to sign in.
In Code, use `/mcp` and the connection belonging to this plugin. Let the user
complete authentication. Do not create a duplicate standalone
MCP entry or request credentials in chat. Verify access with the actual response;
a capability list does not establish the user's account identity.

Discover existing Figma tools before proposing an addition. On a returned access
denial, follow the shared account/existing-connection fallback before asking for
Can edit or reauthentication. Inspect the active host's existing Figma
plugin/connector and MCP routes; prefer a suitable authorized route, not a
namespace. For a needed addition, use the actual host's official Figma integration
and maintained skills. In Claude Code, prefer
`figma@claude-plugins-official`; let the user approve the supported setup in
the selected host. The official remote MCP route is https://mcp.figma.com/mcp;
adding a connection is a separate setup action, not automatic authority from
reading this skill. Follow
[Figma's current setup guide](https://developers.figma.com/docs/figma-mcp-server/remote-server-installation/).

Use actual provider identity/file access evidence to resolve permission issues.
Ask for a file/layer link only when the target is unresolved; keep IDs internal.
Preparation rejoins the existing admission and preview with the user's original
intent and accepted results. Use [the Claude adapter](../../references/claude.md)
for local material and questions.
