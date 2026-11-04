---
name: sambl-setup
description: Prepare or restore Sambl and Figma access in Codex, recover a provider access denial, or resolve the working Figma file before a Sambl design task. Use when the required connection or target is missing, denied or uncertain.
---

# Prepare Sambl access in Codex

Retain the user's task and answers. Read [the selected connection](references/connection.json)
and [external-agent preparation](../../references/external-agent-setup.md), then
continue the requested product skill when its necessary access is ready.
For an installation/MCP health check use sambl-check; kit configuration belongs
to sambl-onboarding or the requested specific product skill.

Reuse the exact installed Sambl environment. When its OAuth session is missing,
use Codex's supported connection/sign-in interface for that server. Check the
actual response; don't infer an account identity from a capabilities list.

Discover existing Figma tools before proposing an addition. On a returned access
denial, follow the shared account/existing-connection fallback before asking for
Can edit or reauthentication. In the Codex app, discover both existing Figma
plugin/app and MCP routes; prefer a suitable authorized route, not a namespace.
For a needed addition, prefer the official Figma plugin and its maintained
skills; offer the host's plugin connection UI when needed, and let the user
complete the access approval.
For Codex CLI the official remote MCP route is https://mcp.figma.com/mcp;
adding it and its skills is a separate supported setup action, not an automatic
change authorized by reading this skill. Follow
[Figma's current setup guide](https://developers.figma.com/docs/figma-mcp-server/remote-server-installation/).

Use the provider's actual identity/file access evidence to resolve an account or
permission issue. Ask for a file/layer link only when the target is unresolved;
keep its IDs internal. Preparation rejoins the existing admission and preview,
with the user's original intent and accepted results. Use
[the Codex adapter](../../references/codex.md) for local material and questions.
