# Auth Shell — product component specification



Named kit dependencies and token paths below are preferred source-parity targets.
For proved absence apply the delivered adapter's general kit-resolution
extension and record the actual compatible bindings/deviations. This never waives
the required Auth Shell anatomy, genuine Main Slot/API, current-mode behavior,
fit or ownership and native evidence requirements, and grants no token/style creation.

## Purpose and artifact

A centered, signed-out shell into which a screen inserts its content. Create
exactly one local COMPONENT named `Auth Shell`, directly under the authorized
`Product Components` native Section. The component root is the `Root` anatomy
role; do not rename the component itself to `Root`. Description Markdown:
`Centered shell for signed-out content.` No ComponentSet and no variants.

This component-only stage creates no Sign In screen, populated default content,
kit primitive, variable, style, prototype/auth service or extra display specimen.
Its target must have zero exact Auth Shell source candidates in the named scope;
existing, partial or ambiguous candidates are conflicts rather than replaceable output.

## Public contract

Exactly one public property, in first/last position: `Main`, type SLOT, empty and
unrestricted. It is a true native Slot, not an instance swap, text property or
Frame. No `Size Class` or other selector property, even when a breakpoint
collection exists. Responsive behavior comes from current token bindings.

Main settings: `displayEmptyByDefault=true`, `stretchChildOnInsert=false`, null
child limits. No new preferred-content list is declared. Create the native Main
Slot first and retain its automatically created SLOT property/key; do not pre-add
a second Main property. Require one Main definition and one true backing, with
`componentPropertyReferences.slotContentId` pointing to that definition.

## Anatomy and binding inventory

| Role | Type and ownership | Layout/sizing | Required bindings and fields |
| --- | --- | --- | --- |
| Root | New COMPONENT named Auth Shell | Vertical; FIXED width × FIXED height | Width/minWidth/maxWidth and height/minHeight below; fill floor-0; clipsContent=true; overflowDirection=VERTICAL |
| Content | New FRAME directly in Root | Vertical; FILL × FILL; primary CENTER, counter CENTER | Inline padding margin-horizontal; both block paddings space/650; minHeight reference height; transparent; clipsContent=false |
| Main | New native SLOT directly in Content | FILL × HUG | maxWidth=600; no padding/gap; empty insertion height=100; clipsContent=true; overflowDirection=NONE; transparent |

Frame defaults unless explicitly overridden: no paint/stroke/effects, zero
padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Main's 600 content cap
and 100 stored empty insertion height are deliberate literals: 100 is not a
minimum height or a new token. No radius is requested.

Resolve each token by exact semantic path AND type in its actual current local
owner; migrated variables may now belong to Core. Names/ids from the reference
file never select destination objects. Bind, do not sample resolved values:

| Exact local path | Type | Target field(s) |
| --- | --- | --- |
| shared-components/main-layout/size/base/root/width | FLOAT | Root width |
| shared-components/main-layout/size/base/root/min-width | FLOAT | Root minWidth |
| shared-components/main-layout/size/base/root/max-width | FLOAT | Root maxWidth |
| shared-components/main-layout/size/base/root/height | FLOAT | Root height and minHeight; Content minHeight |
| shared-components/main-layout/size/base/root/margin-horizontal | FLOAT | Content paddingLeft and paddingRight |
| space/650 | FLOAT | Content paddingTop and paddingBottom |
| colors/layer/floor-0 | COLOR | Root fill |

No typography, icons, media or kit components are inserted into this empty shell.
Do not restore deleted collections/modes or create aliases/tokens to fill a gap.
Current platform/theme are inherited from the authorized environment. See
`../current-context.md` for exact mode semantics.

The Product Components native Section uses current-context.md's supplied
presentation after source geometry settles. Resolve these additional Section-only
tokens: COLOR `colors/layer/floor-1`, FLOAT `stroke/100`, COLOR
`colors/border/neutral-secondary`, FLOAT `radius/200`; smoothing0.6 and inside
stroke. These style the owned Section, not the Auth Shell root/anatomy or a new
Surface. The source's floor-0 fill and other bindings above remain unchanged.

## Lifecycle boundary

All new nodes and Slot definition keys must be recorded as created. Under this
source's narrowly declared cleanup envelope only, at most one proven NEW orphan
SLOT definition per Slot-create operation may be removed: record owner/type/name/
ancestry and exact key at creation; prove zero backlinks immediately before its
removal and one retained intended key/backing afterward. This does not authorize
scratch-node deletion, changes to any pre-existing property, source cloning,
resetting existing output or cleanup by name/prefix. Unknown residue stops the stage.

Use the shared native grouping policy within the provider budget. Verify each
Slot lifecycle group before dependent writes and retain scoped cleanup identities.
Use updated Flexbox-like auto layout; use the current Auto Layout supported by Figma; no migration or version audit is needed.

## Consumer contract for the next stage

Screen content is inserted only into Main. Auth Shell stays linked and its
source stays empty. Root viewport bindings and source anatomy remain unchanged.
The Sign In primary consumer root alone may increase its height under that
screen's explicit fit rule; this permits no descendant geometry patch or source edit.
Root scroll configuration does not prove the populated screen fits.

## Completion evidence

The agent performs the checks in `../acceptance.md` itself. A builder reports exact created
source identity, the single property/backing, bindings, literals and unresolved
provider/UI limitations. API readback is not visual or Inspector acceptance.
