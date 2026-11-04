# Client Cell — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Client Cell as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Set descriptionMarkdown: “Client connection row showing availability and connection status.”

Display name: Client Cell. Exact reference full source API: Layout=Detailed then Compact, each Status=Connected then Coming Soon; default Detailed/Connected. This structural Layout axis is not Size Class. Screen consumers select Compact at sm/md/lg and Detailed at xl using the actual baseline map. Do not infer a tuple from geometry.

## Props

Layout VARIANT Detailed/Compact, default Detailed; Status VARIANT Connected/Coming Soon, default Connected. Preserve these independent structural/status semantics; no Size Class or invented client-content props. Existing nested List/Addon/Rich Icon/Badge APIs remain editable.

## Layers

- Root COMPONENT vertical FIXED × FIXED, initialheight72 literal; initialwidth343 Compact or736 Detailed, FILL-width consumer. Zero gap/padding.
- Linked 💠 Cell Variant=List,Size=Large,Addon Size=Large,Has Start Addon=true,Has End Addon=true, FILL × HUG.
- Start: 💠 Cell Addon Start Size=600,Has Rich Icon=true; Has Icon/Radio/Checkbox/Custom=false. Its Rich Icon Size=600,Shape=Squircle,Has Icon=true,Has Image/Slot=false. Connected uses logo_figma_color and Has Stroke=true in BOTH Compact and Detailed; Layout must not change provider identity. Coming Soon both use logo_chatgpt,Has Stroke=true. selected Dashboard screen contract explicitly selects each client's logo.
- Center: 💠 List Size=600. First List Item600 Has Title=true,Has Value=false,Title=Figma Agent for Connected or ChatGPT for Coming Soon. Second List Item500 Has Title=true,Has Value=false,Title=Mention @Sambl in any copy of the Sambl UI Kit. Has Subtitle=true only Detailed+Connected; false otherwise.
- End: 💠 Cell Addon End600,Has Custom=true; Has Icon/Rich Icon/Button/Checkbox/Radio/Switch/Loader=false. Its true Custom Slot contains 💠 Badge600/Secondary,Has Label=true,Has Slot=false,Has Icon Start=false. Connected: Intent=Positive,Label=Connected,Has Icon End=true,Icon End=checkmark. Coming Soon: Intent=Neutral,Label=Coming soon,Has Icon End=false.

## Variant Order

Detailed/Connected; Detailed/Coming Soon; Compact/Connected; Compact/Coming Soon. First tuple default. Preserve this explicit full source API independently of file mode order. Unknown modes/default replacement require explicit mapped disposition, never invented options or restored axes.

## Default References

Local 💠 Cell List/Large/Large and its native Addon/List dependencies; 💠 Rich Icon600/Squircle; 💠 Badge600/Secondary/Positive and Neutral; local logo_figma_color, logo_chatgpt and checkmark. The selected screen resolves Claude from the exact current default kit local icon component; no external SVG or remote import.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Preserve Cell/Addon/List/Badge/Rich Icon native geometry bindings. No new size tokens. Fixed source72height and343/736authoring widths are source literals, not viewport definitions; parent sets consumer Fill width.

## Typography

Preserve native List Item600 client-title and Badge600 styles. Exact reference Detailed/Connected supporting sentence uses the nested List Item500 Title TEXT with existing compact/300/default, not its default compact/300/accent. Use current local style identity and neutral-secondary binding; Regular400 is a resolved verification, not a raw font setter.

This is a documented Typography/Color consumer override on that exact existing nested Title TEXT, paired with the screen contract. If public/inherited state already supplies the exact result, assert read-only. Otherwise use only the current source-supported Typography/Color route; load actual fonts and preserve linked Client Cell/List/List Item, content/property references, bounds and unrelated bindings. Do not replace the text with Semantic Text, detach, edit kit masters, resize inherited frames or create a style. Unsupported route is a dependent gap.

## Visual Tokens

Connected title `colors/content/neutral-primary`; supporting text `colors/content/neutral-secondary`; Coming Soon title and Badge label use `colors/content/neutral-tertiary`. Connected Badge checkmark follows `components/badge/variants/variant/secondary/intent/positive/layers/content/color`. The Rich Icon Color layer binds colors/layer/floor-2 at full opacity for Connected Figma in BOTH layouts, and for the existing Coming Soon clients. Connected Figma identifying stroke is enabled and binds colors/border/neutral-primary at full opacity in both source variants. The selected screen repeats this rule for actual clients. This paired consumer Color override is permitted by the Rich Icon contract: preserve its shape/mask/dimension bindings and apply only the declared semantic paint on Color. Matching inherited state is read-only. Preserve provider multicolor logo artwork; do not paint atomic sources. Strokes retain source-native topology; selected unavailable clients use the declared neutral-tertiary identifying border through the supported nested Shape Vector paint route. Never retain source remote variable IDs.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Only retained composition closure is built. Resolve native Cell tuple and EndAddon true Custom Slot before inserting a correctly configured Badge. Never clone/swap a populated native Slot dependency. Scenario-specific names/logos modify linked nested properties; do not expose a new top-level client-content API or insert unrelated Empty State/Instruction Step families.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

After combineAsVariants: vertical NO_WRAP HUG×HUG, MIN/MIN; gap/padding16; no fills/effects/styles; solid #9747FF 100% stroke1 INSIDE, dash[10,5], capNONE, joinMITER, miter4; radius5/smoothing0; opacity1, PASS_THROUGH, clipsContent=true. Read back every literal chrome field; never copy another set's chrome. Direct variants retain specified sizing.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.

## Selected Connected consumer outline

The selected screen retains the Connected Figma Rich Icon stroke
Shape Vector bound to colors/border/neutral-primary, resolved opacity1, in BOTH layouts. Preserve all
other stroke/mask/size geometry and native multicolor provider logo. This explicit
consumer paint permission is paired with the screen WHAT; it does not authorize
an implicit source edit. A user-requested existing-source correction needs its own explicit bounded authority and fresh acceptance.
