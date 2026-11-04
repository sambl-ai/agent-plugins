# Navigation — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Navigation as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Navigation`. None. One COMPONENT.

Set descriptionMarkdown: “Navigation region containing a replaceable product menu.”

## Props

`Menu`: true SLOT; default one linked Menu, unrestricted. Non-selector. No Size Class property.

## Layers

- Root COMPONENT: vertical FIXED × FIXED, initial256×812 literal authoring bounds, transparent.
- `Menu`: true SLOT, FILL × FILL, zero padding/gap; contains one source-named Menu instance FILL × FILL.

## Variant Order

None. One COMPONENT.

## Default References

Local product `Menu` COMPONENT with true `Groups` Slot.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

None. Initial256×812 authoring bounds are literals; consumers must set FILL × FILL in the Dashboard Navigation region. Nested Menu fills both axes.

## Typography

None. Menu owns typography.

## Visual Tokens

None. Transparent region; preserve nested styles.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Both Navigation instance and its inserted Menu must fill the available region vertically, including content-tall pages. Do not leave Menu HUG.

Owned Slot settings for Menu: displayEmptyByDefault=true, stretchChildOnInsert=false, null child limits; preserve declared preferred content and descriptions. Create its native backing first and reuse the single automatically created SLOT definition; require one definition and one true backing. For this new owner only, cleanup may also remove at most one proven new orphan SLOT definition per create operation: record its exact definition key, owner id/name/type/ancestry and role at creation; before deletion prove zero backlinks and the retained intended shared key/backings. Preserve every pre-existing definition; unknown residue or another orphan stops. This does not authorize scratch-node deletion.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.
