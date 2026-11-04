# Dashboard — selected screen WHAT

**Dashboard** is an example screen from a product dashboard. Use Dashboard
in screen descriptions, generated root names and result links. Follow the exact
content, structure and behavior below; do not invent charts, metrics or another
screen. Literal navigation, breadcrumb, block and status labels are canvas copy,
not alternate screen names. Dashboard Shell is its product shell component.

Receive this full unit, [exact content](content.md), [component plan](component-plan.md),
[dependencies/style](kit-dependencies.md), [contract deltas](contract-deltas.md),
[current context](current-context.md), [acceptance](acceptance.md), required
consumer API units/assets and byte-pinned generic HOW before dependent writes.
No repository/reference-canvas lookup is an executor prerequisite once approved
complete delivery is available.

## Required outcome and ownership

Create one direct linked Dashboard Shell screen root per actual retained
breakpoint mode, named `Dashboard / {actual mode label}`, in one
selected row of Examples. The Shell owns Root/Main/Navigation construction,
padding, clipping, fills and minimum height. Screen consumers own their name,
actual mode/selector binding, closed navigation/overlay state, selected destination
and prescribed Main/Navigation content only. Do not add a redundant screen Frame,
local fixed-height correction or duplicate compact Nav Bar.

Preserve current platform/theme and bind actual modes/selectors; source variant
inventory never restores modes. Root and immediate Main are content-HUG, with
the current reference height as minimum. Navigation fills resolved Shell height.
Reference dimensions below are observations, not sizing constants:

| Reference baseline | Root observation | Client layout | Workflow collection |
| --- | --- | --- | --- |
| sm | 360×1248 | Compact | HORIZONTAL+WRAP, one visual column |
| md | 600×1088 | Compact | native GRID, two equal FLEX(1) columns, two HUG rows |
| lg | 800×1182 | Compact | native GRID, two equal FLEX(1) columns, two HUG rows |
| xl | 1200×974 | Detailed | HORIZONTAL+WRAP, three equal-width cards |

Only the specified default screen state is selected. No open navigation, Get Started, errors,
loading, pending, clipboard-success, Account or Support screen is constructed.

## Source/API and consumer decisions

Use the self-checked compatible ten-family reference-source closure. Retain
available links and supported public APIs. Main and Overlay source defaults are
empty; reference Navigation defaults contain one linked Navigation in every
source variant, hidden on compact. Do not silently adopt the later portable
empty-default/profile-pruned recipe. The reference-default policy is integrated into Dashboard Shell WHAT; contract-deltas.md records the selected scope and precedence.

Set Is Navigation Open=false and Has Overlay=false. Compact retains its
source-owned Nav Bar and hidden navigation. Wide Navigation/Menu retain their
true Slots, full-height Fill and source identity. Configure the supplied exact
navigation content through supported consumer properties/true Slots; select only
Connections. Never add a screen-name selector to Navigation.

Main's content in exact order:
1. linked Title Block Context=Standard, breadcrumb Connections, heading
   Sambl is ready, no subtitle; retain its own Separator;
2. owned Connections block;
3. one linked horizontal Separator;
4. owned Workflows block.

Preserve available linked root/source identity. Exact-source fidelity is the preferred reference; proved absent dependencies may use suitable replacements under the general shared policy. If a
dependency is proved absent, the shared generic missing-dependency policy applies:
use complete WHAT and current kit variables/available components to supply honest
owned semantics, warn before and after construction, retain remaining links,
declare lost source/API behavior and mark unavailable checks N/A. No fake Slot,
new kit source, import, primitive repair or provider-restriction bypass. Missing required behavior/facts or an unresolvable suitable variable mapping remain real gaps. This does not permit omitting required content or calling an owned Frame the missing linked source.

## Owned blocks and typography

Connections, Workflows, their Text Block wrappers and client List are VERTICAL,
NO_WRAP, FILL width/HUG height, primary MIN/counter MIN, zero padding, transparent,
unstroked/effect-free, clipsContent=false, overflow NONE. Each Text Block is a
zero-gap pair of linked Semantic Text instances: UI Header M heading then Compact S
supporting text. List gap is zero. Connections intro/list gap is space/400;
Workflows intro/items gap is space/600. Full copy is in content.md.

Semantic Text instances FILL/HUG and wrap full paragraphs; preserve their current
variable-driven styles. Page title uses semantic/ui-header-l/accent; block titles
semantic/ui-header-m/accent; supporting copy semantic/compact-s/default; workflow
titles semantic/ui-header-s/accent and descriptions semantic/paragraph-s/default.
Both block supporting lines use colors/content/neutral-secondary. Primary versus secondary/tertiary color roles are in kit-dependencies.md.

Two paired consumer overrides are explicitly permitted by their component WHAT:
- Projects: linked Semantic Text UI Header XS uses semantic/ui-header-xs/default and neutral-tertiary;
- Detailed Figma support: nested List Item500 Title TEXT uses compact/300/default and neutral-secondary.
Regular400 is a resolved check, not a raw font recipe. Preserve linked instance, style role/scale, property references, geometry and bindings. Matching inherited identity is read-only; otherwise use only the supported Typography/Color route, with actual style identity/alias verification. No detach, new style or kit-master edit. An actual provider restriction on an existing object stops that dependent operation; absence may use a suitable existing style/owned composition with warning, preserving required role/rhythm.

## Client rows

Insert exactly Figma Agent Connected, Claude Coming soon and ChatGPT Coming soon.
Select actual native Client Cell Layout/Status tuple before content overrides;
Compact at sm/md/lg, Detailed only at xl. Every row FILL width, native height.
Set nested List Item Title and Has Value=false through current public APIs.

Rich Icon is Size600/Squircle, Has Icon=true, Has Image=false, Has Slot=false:
- Compact Figma: exact local logo_figma_color, Has Stroke=true, native logo colors; existing stroke Shape Vector uses colors/border/neutral-primary at resolved opacity1;
- Detailed Figma: exact local logo_figma_color, Has Stroke=true, native logo colors; existing stroke Shape Vector uses colors/border/neutral-primary at resolved opacity1;
- Claude: exact current kit local recolorable logo_claude, Has Stroke=true;
- ChatGPT: exact local recolorable logo_chatgpt, Has Stroke=true.

Rich Icon Color binds colors/layer/floor-2 at full opacity for all three clients in BOTH layouts. Connected Figma logo/background/outline identity is independent of Layout. Apply only the supported consumer Color-layer semantic-fill override described by Client Cell; preserve shape/mask/size and atomic sources.

Do not infer Layout from a72px height. The earlier Detailed-plus exception is explicitly REVOKED for Connected Figma: use the same provider identity/paint roles as Compact. This is a product correction to the reference reference, not a change to generic Rich Icon defaults.
Supporting Figma sentence appears only in Detailed/Connected. Preserve Badge
Connected positive/checkmark and Coming soon neutral/no end icon. Coming-soon
text, recolorable icon and identifying border use neutral-tertiary without
repainting atomic sources. Reacquire after swaps and verify actual local identity.

Resolve all icon identities from the current default kit by exact local identity/type/ancestry and public swap API. No delivered SVG or external asset import. The avatar in the full retained source APIs uses the current Image component default complete paint/style/reference, an explicit user-approved historical deviation; see avatar-image.md.

Resolve preferred icons locally, or choose a suitable available kit icon when absent under the general policy. Preserve meaning/status and copy; never fabricate/download a brand asset or imply identity fidelity after replacement. If a decorative nonessential icon is omitted, remove any empty spacer and report the omission/lost source parity. Required unresolved functional meaning remains a real gap. No real connection behavior is implemented.

## Workflow collection

Use three linked Workflow Items in exact content order. Each inserted consumer
root has minWidth224 literal and HUG height; source minimum remains unset.
At sm/xl roots FILL width; at md/lg each card also uses native FILL width within its own FLEX Grid column, with HUG height. Width follows the current column when resized.
Never copy sampled224/236/276/328 widths or card heights into new layout. At md/lg use layoutSizingHorizontal=FILL on linked card consumers after they are children of the native auto-layout GRID. FIXED/AUTO at a sampled width is insufficient. Keep one-cell spans and the empty last cell; do not add a resize handler.

Items is FILL/HUG, MIN/MIN, zero padding, transparent, nonclipping:
- sm: HORIZONTAL+WRAP, horizontal gap space/350, row/counter gap space/550;
- md: GRID2×2, FLEX(1) columns/HUG rows, column gap space/350, row gap space/550;
- lg: same Grid, column gap space/450, row gap space/650;
- xl: HORIZONTAL+WRAP, horizontal gap space/550, row gap space/650.

Grid children occupy cells (0,0),(0,1),(1,0), spans1×1; final cell stays empty.
Do not stretch the last incomplete row or replace native Grid with wrapped stacks.
Select source-owned nested Rich Icon/Button APIs; Copy prompt remains static
Default. Source Addons stays hidden/empty; no public API invented.

## Inherited assertions and completion

Root is HORIZONTAL NO_WRAP MIN/MIN, clipping, overflow NONE. Main FRAME is
VERTICAL FILL/HUG, primary MIN, counter MIN at sm and CENTER at md/lg/xl,
nonclipping. Main true Slot is VERTICAL MIN/MIN, FILL/HUG, maxWidth800 literal,
gap space/650; sm overflow VERTICAL, others NONE. Keep source-owned responsive
padding/minima and current bindings. A mismatch is a source/context gap, not
permission for screen-local descendant geometry repair.

Finalize the two native Sections using current-context.md only after geometry
settles. No extra Surface. Perform the affected-scope self-checks, report actual
created/reused sources/roots, declared literals/deviations/warnings and precise
unchecked limitations, then invite the user to view the screen.

## Revised navigation source defaults

The accepted Dashboard Shell must already carry the content.md names/icons in every retained variant, including hidden compact backings. Assembly reuses those defaults and changes only selected destination or explicitly specified consumer content. It must not be the first stage that fixes generic Group/Menu Item/plus placeholders. Source Menu Group title typography is matching-scale Default; Root itemSpacing is space/200 (8), Title padding and Items Slot gap space/50 remain unchanged. Hidden Title leaves no separate gap. No global Semantic Text edit.

## Native Grid assembly order inside Main Slot

For the selected md/lg Grid composition, create the exact retained Shell tuple
first, retain its current mode, selector and sizing bindings, and resolve its
actual consumer Main SLOT through the public property/backlink. Read the real
Slot identity; an ordinary Main FRAME is not that Slot.

Prepare the owned Main composition before Slot insertion. Append the linked
Workflow Items to its owned auto-layout GRID, then configure FILL/HUG consumers,
the existing minWidth224 literal, equal FLEX columns/HUG rows, bound gaps,
one-cell positions/spans and exact nested content/actions. Set the owned Items/Grid
`clipsContent=false` explicitly before Slot insertion; keep it false after insertion.
Do not inherit the new Frame default or change Shell clipping. The Workflow Item
source keeps its FIXED authoring width and unset source minimum.

Insert the prepared content through the supported consumer Slot route. Reacquire
the populated Slot and inserted composition. Apply FILL only to the inserted
composition root when required by its new parent; preserve configured nested
Grid/card sizing. Do not use descendant card width/height setters after insertion
to repair sampled geometry. A provider restriction, wrong identity or invalid
Slot remains a precise gap; do not detach or silently rebuild around it.

Verify each linked card's actual mainComponent identity, ancestry through the
true Slot and page, FILL/HUG sizing, selected tracks/cells/spans and gap aliases.
Read back Grid `clipsContent` and require exact false at each checked width;
include this field in any cross-run comparison. A visually unclipped short text
is not evidence that clipping is disabled.
For an authorized parent-width check, resize only the owned Shell root and observe
automatic equal card widths and text/HUG reflow. Governing bindings stay protected
unless the particular consumer sizing override was explicitly selected. Never
remove a source width alias or change modes to force a test width.

Preserve native Grid in md/lg, the empty last cell, and the specified per-mode gaps and minima. Do not generalize one breakpoint to the others.
