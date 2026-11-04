# Sambl MCP plugin

This package connects to one Sambl MCP environment and bundles skills from the
shared Sambl library, including its service diagnostic, and shared brand assets.
Both Codex and Claude Code builds include local product instructions and access preparation.
It contains no server runtime or credentials. Sign in through the host's MCP
OAuth flow under your own account.

| Environment | MCP name | Diagnostic skill |
| --- | --- | --- |
| local | sambl-local | sambl-check |
| dev | sambl-dev | sambl-check |
| production | sambl | sambl-check |

The diagnostic checks installation and connectivity; product workflows belong
to their own canonical product entries.
Use the diagnostic matching this plugin. It reads its bundled connection reference
and never falls back to a different Sambl environment. `SAMBL_PLUGIN_SKILL_OK`
confirms the skill loaded; `SAMBL_MCP_OK` confirms a real capability call;
`SAMBL_MCP_UNAVAILABLE` reports the observed connection/sign-in/request failure.
No Figma file or writer is needed, and no file contents are changed.

Skill names are the same in every environment. In Codex, select the plugin's
namespace explicitly: `$sambl-local:sambl-check`, `$sambl-dev:sambl-check` or
`$sambl:sambl-check`. Other library skills keep their source names too.

In both hosts, `sambl-setup` prepares missing access or resolves the working file and
then resumes your original task. It is available without a mandatory MCP
dependency. Sambl MCP authorization, the Figma native connection/file permission
and Sambl's Figma REST access are separate. Setup reuses working connections;
connection approval does not replace the product's preview and Apply decision.
Use `sambl-onboarding` to configure the kit itself.

The current product release for both hosts has 11 user entries for help, onboarding, Slot
defaults, Themes, Platforms, Size Class, Collections, Palette, semantic colors,
Examples and feedback. Three internal skills for variable creation and Examples
construction are supporting references. Continuous and separated light-surface
recipes and Sign In/Dashboard specifications are included; Typography is not
included. These counts describe the package scope, not an extension limit.
`sambl-check` and `sambl-setup` are
additional service entries.

Product instructions come from one canonical connector package, also delivered
remotely to Figma Agent. Read the complete local references through
`references/reference-index.json`; it pins their versions and this package's
Sambl connection. Do not refetch an already loaded static entry. Live capability
discovery, recognition where required, calculations, proposals, reporting and
feedback still call that Sambl MCP. Examples obtains its actual catalogue and
packageVersion through `get_example_package`; local material must match it.

`references/product-manifest.json` records source and product-file integrity;
it does not establish access, authorization or live acceptance, and does not cover
every package file. Plugin semver and canonical reference versions are distinct.
On a revision mismatch, update/reconcile the matching package and server instead
of mixing instructions or repeating completed changes. Changes shared by local
instructions and remote phases require a coordinated server/local release because
remote phase instructions are supplied by the server.

From the private clone, `pnpm dev:plugin:codex --environment <environment>` builds,
installs and launches OAuth; `pnpm update:plugin:codex --environment <environment>`
updates only that environment. Root .env.dev (default), .env (local) and .env.prod own configuration.
See `plugin/LOCAL-DEVELOPMENT.md` for environment selection,
port 3010 for local Docker, production naming and update steps.

A prebuilt local installation uses the separate environment-specific marketplace.
Uploading only the ZIP via New plugin saves it privately to the OpenAI account;
that differs from a disk-only installation. The ZIP itself has no catalogue.

For Claude, `pnpm dev:plugin:claude --environment <environment>` builds and
installs through a separate local marketplace; `pnpm update:plugin:claude` updates
it (keep the selected environment). The installer adds a content-derived local
version suffix so changed skills refresh without manually clearing Claude's cache.
It installs into Claude Code and, with an active Desktop profile, separately into
its local Cowork marketplace store. In Desktop, reopen Settings → Plugins → Yours
(reload the window if cached) and select Connect on the plugin's Sambl connector.
The installer verifies plugin files and leaves MCP authentication manual.
In Code, use `/reload-plugins` or start a new session, view the plugin through
`/plugin` and sign in through `/mcp`. Desktop chat needs its separate
Connect flow. Invoke `/sambl-dev:sambl-check`, `/sambl-local:sambl-check` or
`/sambl:sambl-check`. Product and setup skills use the same plugin namespace.
A session-only build can be loaded with `claude --plugin-dir <package-directory>`.

Known OAuth compatibility issue: Hydra DCR responses with `client_uri: ""` or
`contacts: null` can fail Claude's strict MCP SDK parsing before the sign-in
browser opens (`Invalid URL` / `expected array, received null`). Successful
installation does not resolve this authentication issue. See
[Hydra #4116](https://github.com/ory/hydra/issues/4116) and
[Hydra #4044](https://github.com/ory/hydra/issues/4044).

Local build/contract checks do not establish live Codex/Figma use or Codex Cloud
readiness. Installation, OAuth and actual file outcomes need their own validation.
