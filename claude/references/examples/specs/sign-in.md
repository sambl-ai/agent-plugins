# Sign In / Default — screen specification



The adapter's general kit-resolution extension governs proved absence of
named preferred components/styles/tokens/media in this WHAT. Verify actual chosen
alternatives and bindings; disclose exact-source/API/visual differences as N/A
parity checks. Required copy, semantics, functional native behavior, fit and stage
acceptance remain required. No component-specific fallback list is introduced.

## Selected scope and prerequisites

Only Sign In / Default, scenario `sign-in`, across ALL actual retained modes and
current platform/theme. Exactly one required product family: Auth Shell. No
Dashboard, Navigation, Main Layout, account, loading or error screen is in scope.
Build the required Auth Shell first when absent; reuse it when compatible, then preserve its source while assembling the screen.
Handle absent dependencies by their documented roles; unread/ambiguous/defective
or restricted existing sources are distinct gaps, not proven absence.
Do not clone or inspect the reference Examples for construction. Resolve current
kit sources and live token bindings from the local target.

## Exact visible content

| Role | Exact text |
| --- | --- |
| Heading | Welcome to Sambl |
| Description | Use your Figma account to access Sambl and manage your connections. |
| Button label | Continue with Figma |
| Legal | By continuing, you agree to the Terms of Service and acknowledge the Privacy Policy. |

Use the exact legal ranges `Terms of Service` and `Privacy Policy` for link-style
color only. They are inert text; no URLs, hyperlinks or navigation are required.
This static example does not execute authentication or imply current legal acceptance.
Authoring status/scope/provenance notes are never visible content.

## Anatomy and reading order

The screen root is a linked Auth Shell instance, directly under Examples, with
its source-inherited internals preserved. No Main Layout or redundant screen Frame.

```text
Auth Shell instance = screen root
  inherited Content
    inherited Main [true SLOT; source remains empty]
      Content [owned transparent wrapper]
        Card [presentation role; preferred linked 💠 Board]
          Items [content group; true SLOT when using linked Board]
            Brand identity [preferred linked logo_sambl_color]
            Text Block [owned transparent wrapper]
              💠 Semantic Text / UI Header L [heading]
              💠 Semantic Text / Compact M [description]
            Actions [owned transparent wrapper]
              💠 Button [Continue with Figma]
        💠 Semantic Text / Compact S [legal, OUTSIDE card]
```

The inserted Content wrapper is vertical FILL × HUG, maxWidth600 literal,
gap bound to space/400, zero padding, no fill/stroke/effects, clipsContent=false.
The Content wrapper is centered by Auth Shell's existing Content parent.
The card role is vertical FILL × HUG, primary MIN / counter CENTER, gap0, with one
vertical FILL × HUG items group, primary MIN / counter CENTER, zero padding, no
paint/stroke/effects, clips=false/overflow=NONE. Order: logo → Text Block → Actions.
The role's complete visual fields and responsive token mapping are below.
Retain matching linked-source alignment as a read-only assertion; no alignment
override is authorized. Screen-owned Card and Items use these same alignments.
Prefer available linked Board: its Items is a true Slot; retain its identity,
backlink/settings/preferences and matching inherited geometry, and populate only
the consumer content. When the role is composed from owned native layout instead,
card and items group are ordinary FRAMEs named `Card` and `Items`; they claim no
Board source/API, SLOT property/backlink/preferences or future source updates.
This representation decision belongs to the generic assembler, not a named
missing-Board branch. No additional surface or third wrapper is part of the role.

Text Block: vertical FILL × HUG, zero gap/padding, transparent, no stroke/effects,
clipsContent=false. Its linked heading precedes linked description.
Actions: vertical FILL × HUG, primary MIN / counter MIN, zero padding,
transparent, no stroke/effects, clipsContent=false, gap from the responsive table.
Keep inherited names on all nested kit instances; role names above label only
newly owned wrapper nodes.

## Required fields and linked-source override inventory

| Target | Inherited field to retain | Required consumer change |
| --- | --- | --- |
| Auth Shell primary root | Source, width/min/max/minHeight bindings; clips=true; overflow=VERTICAL | Assign exact actual size-class mode where present; height may grow only under fit rule below |
| Auth Shell inherited Content | FILL × FILL, centered, inline/block paddings and minHeight bindings, transparent and unclipped | None |
| Auth Shell Main true Slot | Identity/backlink/settings, FILL × HUG, maxWidth600, clips=true, overflow=NONE | Populate consumer override only; source stays empty |
| Card role | Linked Board identity when available; primary MIN / counter CENTER; no effects; clips=false; overflow=NONE | FILL × HUG; fill floor-1; all corners radius/700, smoothing0.6; all border widths stroke/400, solid border paint neutral-primary; strokeAlign=INSIDE; strokesIncludedInLayout=false; responsive padding below. On owned FRAME composition these are bound role fields, not inherited overrides. |
| Items content group | On linked Board: true Slot identity/backlink/settings/preferences; vertical FILL × HUG; MIN/CENTER; zero padding | Gap bound to exact responsive token; ordered content. On owned composition use an ordinary FRAME with those fields, no Slot/API claim. |
| Brand identity role | Prefer exact linked local color logo with full authored colors and locked square aspect | For that source bind governing width below and derive height; do not bind second dimension or unlock aspect. Proved absence follows the shared semantic identity substitution rule, with existing variable/text-style bindings and disclosed visual/source difference. |
| Semantic Text instances | Exact style identities/property references; internal rhythm and layer geometry | Text and hidden Slot booleans; semantic fills; current consumer TEXT paragraph formatting below |
| Button action role | Preserve available linked exact source/tuple and internals | Exact label and API values below, FILL × HUG. Figma start decoration is optional; when available it uses exact logo_figma_color. |

Here floor-1 means exact COLOR `colors/layer/floor-1`; border neutral-primary means
`colors/border/neutral-primary`, NOT content neutral-primary. Do not substitute
Board's overlay/default radius/padding/gap/absent border.

## Responsive selection

Select by the VERIFIED composition baseline from `current-context.md`, not width,
display label or a guessed variant name. Resolve each binding from current local
variables; literals in token names are not pixel values.

| Consumer field | sm/md baseline | lg/xl baseline |
| --- | --- | --- |
| Card paddingTop | space/650 | space/750 |
| Card paddingLeft/right/bottom | space/450 | space/750 |
| Items group itemSpacing | space/450 | space/550 |
| Actions itemSpacing | space/300 | space/350 |
| logo_sambl_color governing width | size/600 | size/900 |
| Button public Size | 600 | 700 |

When Board is available, Items gap binding is the sole required inherited Items
layout change. Source AND page recipe explicitly permit it. Matching inherited sizing, padding
and alignment are read-only checks, not writes. An explicit provider restriction
stops without workaround; report target/field/error. Do not infer an itemSpacing
ban from an unrelated field restriction. Untested capability remains unverified.

## Typography and colors

Each of heading, description and legal is a linked Semantic Text, FILL × HUG,
Has Slot Start=false and Has Slot End=false, using the complete matching copy.
Load current fonts before existing consumer TEXT paragraph-format overrides:
textAlignHorizontal=CENTER, textAutoResize=HEIGHT, textTruncation=DISABLED,
maxLines=null. This does not authorize moving/reparenting/resizing inherited
frames, changing their auto-layout alignment or inventing Align/Wrap properties.

Preserve these exact existing text-style identities and inherited rhythm:
- Heading Style=UI Header L → semantic/ui-header-l/accent;
  fill colors/content/neutral-primary.
- Description Style=Compact M → semantic/compact-m/default;
  fill colors/content/neutral-secondary.
- Legal Style=Compact S → semantic/compact-s/default;
  fill colors/content/neutral-secondary, with only the two exact legal ranges
  bound to colors/content/brand-extra-secondary as inert link-style text, with no hyperlinks.

The action is a static sign-in affordance labelled exactly `Continue with Figma`.
No OAuth execution/service is part of this specimen. A visible Figma brand icon
is nonessential decoration: the exact text and intended static action semantics
remain without it. Do not fabricate a replacement asset or reserve an empty icon
spacer. Use available component visibility controls and its normal layout.

The available Button uses FILL × HUG, Label=Continue with Figma, Variant=Primary,
Intent=Neutral, State=Default, Has Label=true, Has Icon Start=decoration visibility
(true when supplied, false when omitted),
Has Icon End=false, Has Slot=false, Is Focused=false, and the responsive Size.
The preferred illustrated representation uses exposed Icon Start=exact current
local logo_figma_color with authored colors. Apply the general extension when a
preferred dependency is absent; no invented brand identity, empty spacer or
undisclosed substitution. An allowed omission uses the public visibility API,
retaining hidden default internals. Preserve available Button source-owned
variable-driven typography/colors/spacing/radii; no literal inset/width patch.
No other state/action/specimen is requested.

## Fit and clipping

Center while content fits; allow content-driven height growth with current
reference width, min/max width, minimum height and safe padding retained.
On the PRIMARY screen-instance root only, settle height to the greater of the
current reference/minimum height and resolved Main content height plus both
Content block paddings (space/650 each). Retain height binding when it fits;
necessary growth may replace only that consumer root's height binding with the
computed content-fit height. No sampled viewport/text-height constants.

Preserve Root clipsContent=true / overflowDirection=VERTICAL and Main
clipsContent=true / overflowDirection=NONE; Content stays transparent/unclipped.
Reacquire settled geometry after content/property writes. Full specified content
must fit without clipping. Scroll configuration and root dimensions alone do not
prove this. No inherited-descendant geometry patch or source mutation is allowed.

## Final artifact boundary

Follow `current-context.md` for N roots, current modes, row positions and two
native Sections. Style/finalize Sections last; no extra board Surface. One final
selected-scope check uses `acceptance.md`; no whole-file census. Report actual
representation/omission and source-parity deviations with missing-dependency
warnings before construction and in the terminal report. Report complete,
partial or failed honestly with exact unsupported/unverified fields. Stop after
this screen; do not automatically start another example or an unrelated screen.
