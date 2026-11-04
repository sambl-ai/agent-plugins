---
name: sambl-check
description: Check whether the installed Sambl plugin skill loads and whether its Sambl MCP connection responds, without opening or changing a Figma file.
---

# Sambl Plugin Check

First report `SAMBL_PLUGIN_SKILL_OK`: this confirms that these packaged
instructions loaded. It does not confirm server connectivity or authentication.

Read `references/connection.json` bundled with this skill. Report its environment,
server name and URL, and use only that MCP connection. If several Sambl
environments are installed, never fall back to another one when this connection
is missing or fails.

Then find `get_capabilities` on that exact Sambl MCP connection. Call it using its
published input schema and omit file identity. No Figma file or writer is needed.
If the response has `status: ok`, report `SAMBL_MCP_OK` and briefly describe the
capabilities actually returned. Report an empty catalogue as an empty catalogue.

If the tool is missing, authentication is required, or the request fails, report
`SAMBL_MCP_UNAVAILABLE` and the observed reason. Explain the host's connection or
sign-in step when it is known. Do not infer success from plugin installation,
request credentials in chat, or call file-changing tools for this check.

Use the user's language around these diagnostic markers.
