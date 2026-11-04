# Workflow Item — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Workflow Item as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Workflow Item`. None. One COMPONENT.

Set descriptionMarkdown: “A suggested workflow with explanatory content and a copy-prompt action.”

## Props

None. No Size Class property or invented Title/Description API. Configure existing nested Semantic Text, Rich Icon and Button properties in each scenario instance.

## Layers

- Root COMPONENT vertical FIXED × HUG, initialwidth212 literal, gap space/200.
- Linked 💠 Rich Icon Size=200,Shape=Squircle,Icon=sparkle,Has Icon=true,Has Image=false,Has Stroke=false,Has Slot=false.
- `Content`: vertical FRAME FILL × HUG, zero gap/padding, clipsContent=true; two source-named 💠 Semantic Text instances FILL × HUG: Style=UI Header S then Paragraph S, both Text=Text, both Has Slot Start/End=false. Follow with hidden empty `Addons` FRAME, fixedwidth384, storedheight100, vertical HUG, clipsContent=true; no public prop.
- Linked 💠 Button Size=300,Variant=Secondary,Intent=Neutral,State=Default,Has Label=true,Label=Copy prompt,Has Icon Start=false,Has Icon End=true,Icon End=copy,Has Slot=false,Is Focused=false; HUG × HUG.

## Variant Order

None. One COMPONENT.

## Default References

Local 💠 Rich Icon200/Squircle; 💠 Semantic Text UI Header S and Paragraph S; 💠 Button300/Secondary/Neutral/Default; local sparkle and exact current kit local copy icon.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Bind Root gap Core FLOAT `space/200`. Preserve exact native Rich Icon and Button size bindings. Consumer width comes from the scenario's actual grid column or wrapping row, not fixed212 across all modes. The source minWidth is unset. The selected Dashboard contract explicitly permits minWidth=224 literal on each inserted consumer root only, with HUG height; all retained consumer roots FILL width; md/lg follows its current FLEX Grid column. Do not write this minimum into the source or inherited descendants.

## Typography

Inherited Semantic Text UI Header S and Paragraph S, each Fill width and left aligned. No local text style creation.

## Visual Tokens

Bind Rich Icon's visible Color surface COLOR `colors/background/brand-extra-high` and its sparkle consumer Vector `colors/content/on-brand-extra`; the black Shape Vector is a mask, not a color override. Header Semantic Text uses `colors/content/neutral-primary`, paragraph `colors/content/neutral-secondary`. Swapped Button copy Vector uses existing `components/button/variants/variant/secondary/intent/neutral/layers/content/color`. Preserve other linked kit paints and do not repaint atomic sources.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Source has no responsive variants. The surrounding workflow collection owns columns and gaps. Keep zero-gap Content text block; all actual workflow titles/descriptions come from the selected Dashboard contract. Copy action is a static design affordance here, not a clipboard service or new motion implementation.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.

## Screen consumer width in native Grid

When the selected screen places this linked consumer in a FLEX-track native
auto-layout GRID, FILL width follows its own current column, while height stays
HUG. Keep the selected screen's cell/span/minimum rules. A sampled FIXED width
is not a responsive column binding. This consumer setting does not change the
component source's own sizing or expose a new public property.
