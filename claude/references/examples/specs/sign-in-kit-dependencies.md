# Sign In — local kit consumption contracts



## Required dependency closure

| Exact identity | Type / required supported API | Sign In usage |
| --- | --- | --- |
| Auth Shell | local single COMPONENT; Main true SLOT only | One linked screen root per actual mode; source is read-only after its self-check |
| Card presentation | Preferred source 💠 Board: local single COMPONENT; Items true SLOT, no axes | Use available linked source. The complete card/items semantic layout/token contract is in sign-in.md and remains the required role when the source is absent. |
| 💠 Semantic Text | local COMPONENT_SET; Style variant; Text text; Has Slot Start/End booleans; Slot Start/End true Slots | Styles UI Header L, Compact M, Compact S |
| 💠 Button | local COMPONENT_SET; Size/Variant/Intent/State variants; listed booleans/text/swaps below | Size600 or700 / Primary / Neutral / Default |
| Brand identity | Preferred exact current local retained full-color logo_sambl_color | Preserve its linked source, governing width and square aspect when available; a proved missing source uses the shared semantic identity substitution rule. |
| Figma start decoration | Preferred: exact current local full-color logo_figma_color | Optional decoration on the static action; general resolution policy applies without invented brand identity, with exact label/semantics retained. |

Resolve actual component ids/keys locally; this document intentionally supplies
no historical destination ids. The brand identity's semantic meaning is required;
its preferred graphic is resolved under delivery.md's general substitution policy,
with any visual/source-parity difference disclosed. Figma start decoration is
optional. When using a logo source, names/appearance alone do not
establish local identity or correct source ancestry. No packaged
media, Image placeholder, avatar or network asset is needed by this scenario.
Board's picker recommendations do not add List/Cell/Accordion to the product
build closure: those kit sources remain read-only metadata dependencies.

## Available Board defaults vs permitted consumer overrides

Canonical Board defaults: one COMPONENT, root vertical FIXED × HUG when directly
on a page, reusable consumer may be FILL width; Root contains only Items. Root
fill colors/overlay/neutral; padding space/350 all sides; radius/550 with 0.6
smoothing; no stroke/effects; clipsContent=false. Items is vertical FILL × HUG,
primary MIN / counter CENTER, zero padding, gap space/350.

One public `Items` native SLOT, empty and visible by default:
`displayEmptyByDefault=true`, `stretchChildOnInsert=false`, null child limits.
Accepted recommendations are local List, Cell, Accordion in that order;
`allowPreferredValuesOnly=false`. Keep current settings, definition/backlink,
preferences and other metadata unchanged. No source-default mutation is permitted.

The canonical consumer API explicitly permits background, padding, item gap,
radius and optional border customization with compatible shared variables.
`sign-in.md` supplies the REQUIRED overrides; Board defaults do not satisfy that
recipe. Its only Items layout write is the documented itemSpacing binding;
matching inherited layout/sizing/padding/alignment fields are read-only assertions.
Use a provider-supported consumer route. An explicit restriction stops the
operation; do not probe around it, detach, alter the primitive or introduce a wrapper.
An untested route is an unverified gap, not an observed provider failure.

## Semantic Text consumption

Required public values: Style=`UI Header L`, `Compact M`, `Compact S`; Text is the
existing shared text property; Has Slot Start=false, Has Slot End=false.
All variants have direct children Slot Start, Text, Slot End. Preserve both true
Slots and shared property references. These adjacent Slots stay empty/hidden.
The existing Root is horizontal, FILL × HUG, counter CENTER, gap0, with
component-owned block rhythm; its Text is FILL × HUG. Do not remove root rhythm
or replace a Semantic Text with raw text.

Required existing style identities are:
- UI Header L: `semantic/ui-header-l/accent`.
- Compact M: `semantic/compact-m/default`.
- Compact S: `semantic/compact-s/default`.

Keep style identity and variable-driven font metrics, even when applying a
permitted existing TEXT paragraph-format override. The screen recipe requires
center paragraph alignment, HEIGHT auto-resize, truncation DISABLED, maxLines=null
on that current consumer Text after its fonts are loaded. This is paragraph
formatting, not x/y, layer alignment, resizing/reparenting inherited frames or a
new Align/Wrap component property. Preserve all linked internals and rhythm.
Apply the screen's semantic content fills without replacing styles with sampled
font values. Legal ranges are deliberately inert link-style text; their exact
range fills are required, real URLs/hyperlinks are not.

## Button consumption

Required exact native tuple: Size=`600` or `700`, Variant=`Primary`,
Intent=`Neutral`, State=`Default`. Size is independent from Size Class.
Set Label=`Continue with Figma`; Has Label=true; Has Icon Start=true when showing
the available optional start decoration, false when absent;
Has Icon End=false; Has Slot=false; Is Focused=false. Exposed Icon Start is
INSTANCE_SWAP; use the locally resolved `logo_figma_color` source when present.
For the preferred available decoration use its verified identity. Any compatible
current-kit substitution follows the general extension and public swap API;
disclose the difference without claiming reference-brand/source parity. Omission
uses the public visibility API and leaves hidden default internals unchanged;
do not insert a spacer or change source styling.
Preserve the unused Icon End/Slot/default internals and their public identities.
Button is FILL × HUG at the instance root; there is no Width variant axis.

No Loading/Hover/Pressed/Disabled/focus specimen, spinner or new prototype service.
Icon assets with `_color` retain authored colors. Do not recolor their vectors,
sample a replacement, or override Button's own typography, spacing or radius.

## Shared-token closure for the screen

Auth Shell's exact bindings are in `components/auth-shell.md`. Additionally resolve these
existing paths by exact type/current owner, including after collection migration:

- FLOAT: space/400, space/650, space/450, space/750, space/550,
  space/300, space/350, radius/700, stroke/400, size/600, size/900;
  Section chrome also uses stroke/100 and radius/200.
- COLOR: colors/layer/floor-1, colors/content/neutral-primary,
  colors/content/neutral-secondary, colors/content/brand-extra-secondary,
  colors/border/neutral-primary, colors/background/neutral-high;
  Section chrome also uses colors/border/neutral-secondary.
- Current size-class STRING selector/context only when actually present or
  verified migrated evidence requires it; follow `current-context.md`.

Only require responsive rows used by actual baselines; do not repair removed
modes or fuzzy-match obsolete `shared-components/main-layout/size/root/...` paths.
No copied HEX, pixel font size, new primitive library or new shared row is
authorized. Owned replacement elements are allowed only by the shared substitution
policy and must use suitable existing variables/text styles.
