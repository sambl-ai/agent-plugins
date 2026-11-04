# Dashboard — selected screen content

Only labeled strings below belong on canvas. Scope notes, warnings, source
provenance and testing instructions are not UI text.

## Screen context

- Root display name: `Dashboard / {actual mode label}`.
- Use Dashboard in screen descriptions and result links. The literal interface
  labels below are canvas content, not alternate screen names.
- Breadcrumb: `Connections`.
- Page title: `Sambl is ready`.
- No page subtitle.
- Compact menu closed; Has Overlay=false. No open-navigation, Get Started,
  loading, error, pending, clipboard-success or additional screen specimen.

## Navigation (Dashboard Shell source preset, including hidden compact backings)

Configure these names/icons in the Dashboard Shell source, not only during screen assembly. Generic Menu/Navigation remain generic. Check all retained Shell variants, including hidden compact defaults. Screen-owned selection may override the preset without rewriting source defaults. Preserve the current footer/Image values.

First untitled group:
1. `Connections`, selected, State=Default, local `sparkle`.
2. `Support`, unselected, State=Default, local `question-mark`.

Second group: title `Projects`; one `Coming soon...` item, unselected,
State=Disabled, local `folder-open`. Footer Account Item: `Bo Gydza`,
unselected, State=Default. Preserve Sambl identity. No project rows or routes.

## Connections block

Heading: `Connections`
Supporting text: `Use Sambl with:`

| Client | Status label | Supporting text |
| --- | --- | --- |
| Figma Agent | Connected | `Mention @Sambl in any copy of the Sambl UI Kit` only in Detailed/xl |
| Claude | Coming soon | none |
| ChatGPT | Coming soon | none |

One linked Client Cell per row, in that order. Compact at sm/md/lg; Detailed at
xl. Explicit status text remains visible; unavailable clients are informative,
not live connection controls.

## Workflows block

Heading: `Workflows`
Supporting text: `Choose a workflow, then run it in Figma Agent.`

| Title | Description | Action |
| --- | --- | --- |
| Set up your Sambl Kit | Choose the themes, platforms, and breakpoints your product needs, then customize your kit’s colors. | Copy prompt |
| Update the palette | Provide your main product colors, and Sambl will generate a palette for your kit’s components. | Copy prompt |
| Stay up to date | See what changed in Sambl and which updates may apply to your customized copy. | Copy prompt |

Keep exactly these three cards and exact punctuation/case. Their actions remain
Default static design affordances. No actual clipboard payload or service is
provided by a static Figma example; do not invent executable prototype actions.
The current catalog prompt values are `@Sambl set up my UI kit`, `@Sambl change my palette`, and `@Sambl show the changelog`, respectively. Preserve these values in descriptions where the source API supports them; labels remain Copy prompt.
## Human-selected kit substitutions

All icons resolve from the current default kit; no external SVG imports. The
avatar in the retained product-source API uses the current Image component default
picture with its complete paint/style/reference settings instead of the reference
personal avatar. This is an explicit human-approved historical deviation. If any
preferred dependency is absent, a suitable available kit icon/style/token/component
or honest owned variable-backed composition follows the shared general policy,
with warnings and lost source/API parity disclosed; exact copy/status meaning stays.
