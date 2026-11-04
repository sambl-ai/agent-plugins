# Menu Group — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Menu Group as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Menu Group`. None. One COMPONENT.

Set descriptionMarkdown: “A named group of navigation items.”

## Props

Ordered props: `Has Title` BOOLEAN=true, then `Items` SLOT with two default Menu Item instances. Items preferred values only: exact local Menu Item COMPONENT_SET. Both properties are non-selectors; Has Title controls Title wrapper visibility. No Size Class property.

## Layers

- Root COMPONENT: vertical FIXED × HUG, initialwidth366 literal, paddingTop space/200, root itemSpacing space/200 (8).
- `Title`: FRAME FILL × HUG, inline padding space/200; visibility bound to Has Title. Contains source-named 💠 Semantic Text Style=UI Header XS,Text=Group,Has Slot Start=false,Has Slot End=false, FILL × HUG.
- `Items`: true SLOT FILL × HUG, gap space/50; two source-named Menu Item instances Is Selected=False,State=Default, FILL × HUG.

## Variant Order

None. One COMPONENT.

## Default References

Local product Menu Item; local kit 💠 Semantic Text with UI Header XS and Text/Has Slot Start/Has Slot End properties.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Bind Root paddingTop, Root itemSpacing and Title inline padding Core `space/200`; Root itemSpacing resolves to8 between visible Title and Items. Items Slot gap remains Core `space/50`; do not make it8. Preserve Semantic Text's existing responsive rhythm.

## Typography

Keep linked Semantic Text Style=UI Header XS and its responsive rhythm/API. The Menu Group source title itself must use the existing matching-scale semantic/ui-header-xs/default characteristic, including all existing typography variable bindings. Do not inherit accent and defer this correction to a screen consumer. The Projects consumer additionally uses neutral-tertiary. Regular400 is resolved evidence, not a literal font recipe. Preserve the global Semantic Text source and its defaults.

If exact style/color already inherit, do not write. Otherwise this source/consumer contract permits only that linked Semantic Text consumer's supported Typography/Color override, preserving Style, Text references, Slot API, rhythm, geometry and other bindings. No detachment, master edit, new style or property. Reacquire and verify exact current style identity/bindings; restriction or ambiguous style is a precise dependent gap.

## Visual Tokens

None. Owned wrappers transparent; linked Semantic Text retains semantic content color.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Set Root itemSpacing=8 through the existing space/200 alias, not a new variable or literal-only setting. This separates Title from Items; do not increase Title padding or Items Slot gap. Has Title=false collapses only Title; Items remains discoverable and no separate spacer or empty8px interval remains. The scenario owns actual menu item content and selection. Do not create a group Title text property that was not specified.

Owned Slot settings for Items: displayEmptyByDefault=true, stretchChildOnInsert=false, null child limits; preserve declared preferred content and descriptions. Create its native backing first and reuse the single automatically created SLOT definition; require one definition and one true backing. For this new owner only, cleanup may also remove at most one proven new orphan SLOT definition per create operation: record its exact definition key, owner id/name/type/ancestry and role at creation; before deletion prove zero backlinks and the retained intended shared key/backings. Preserve every pre-existing definition; unknown residue or another orphan stops. This does not authorize scratch-node deletion.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.

## Revised root-gap acceptance (owner request,2026-10-16)

Require Root itemSpacing=8 bound to the current unique FLOAT space/200, retained
Root paddingTop and Title inline padding, and Items true Slot itemSpacing still
bound to space/50. With Has Title=true the8px gap lies between Title and Items;
with false Title is hidden and no independent gap/spacer remains. Existing Slot
API/preferred content, Default typography, item order/selection and unrelated
overrides are preserved. This new repo contract is not live repair authority or
acceptance of older sources; no executed snapshot is rewritten.
