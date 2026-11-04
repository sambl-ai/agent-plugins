# Account Item — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Account Item as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Account Item`. Direct-child order: Is Selected=False,State=Default; Is Selected=False,State=Hover; Is Selected=True,State=Default. First tuple default. Do not create selected Hover combinations.

Set descriptionMarkdown: “Account navigation item showing the signed-in identity.”

## Props

Order: `Is Selected` VARIANT False/True, default False; `State` VARIANT Default/Hover, default Default. Is Selected maps selection=unselected/selected; State Default omits interaction selector, Hover→interaction=hover. Only tuples in Variant Order exist. No other public props, Slots or Size Class axis; nested kit properties remain editable.

## Layers

- Root COMPONENT: vertical FIXED × HUG, initialwidth334 literal, inline padding space/200, block padding0, gap0, corners radius/300.
- Linked 💠 Cell Variant=List,Size=Medium,Addon Size=Small,Has Start Addon=true,Has End Addon=false, FILL × HUG. Preserve native Content Slot/default structure.
- Its 💠 Cell Addon Start Size=300: Has Radio/Has Checkbox/Has Custom=false; Has Rich Icon=true,Has Icon=false. Nested Rich Icon Size=150,Shape=Circle,Has Image=true,Has Icon/Has Stroke/Has Slot=false; the complete current local Image component default paint in avatar-image.md as its Image fill.
- Its 💠 List Size=500,Has Subtitle=false; primary 💠 List Item Size=500,Has Title=true,Title=Bo Gydza,Has Value=false. Keep hidden secondary List Item at its native default; do not manufacture hidden UI kit internals.

## Variant Order

Direct-child order: Is Selected=False,State=Default; Is Selected=False,State=Hover; Is Selected=True,State=Default. First tuple default. Do not create selected Hover combinations.

## Default References

Local 💠 Cell List/Medium/Small with its local Addon/List family; 💠 Rich Icon150/Circle and the complete current local Image component default paint in avatar-image.md.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Root inline padding→Core FLOAT `space/200`; all four corners→Core FLOAT `radius/300`, smoothing0.6. Preserve Cell's exact shared Medium/Small geometry and native nested style bindings.

## Typography

Preserve 💠 List Item's exact native Size500 typography. Content customization uses its Title/Has Value properties, not raw text layer recreation.

## Visual Tokens

Default unselected Root transparent; Hover unselected and Selected Default Root fill→COLOR `colors/overlay/neutral`. Visible title→`colors/content/neutral-primary`. No separate opacity scaling. Apply consumer-level paint bindings without editing atomic sources.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Select native Cell tuple before customizing its nested props. The avatar uses the same complete current Image default-paint contract as Title Block. Read back source/instance name inheritance and preserved hidden dependency defaults. Parent state changes must preserve edited nested content; do not put the adaptive selected/disabled content inside a new product Slot.

Avatar override: receive the complete [current Image default contract](../avatar-image.md). Resolve the exact current local Image component and capture its entire default fill array, paint attributes, style identity/reference and image reference. Reuse that complete current default picture/paint on this linked Rich Icon consumer Image through the supported image-fill route, preserving receiving geometry/mask/stroke and provider badge. Matching inherited state stays read-only. Verify full equality to the captured current default after writes; IMAGE presence or hash alone is insufficient. Do not use the historical personal avatar, bundled bytes, network media, invented photo/style or kit source mutation. Missing/ambiguous current Image identity or unsupported consumer application is a precise dependent gap.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

After combineAsVariants: vertical NO_WRAP HUG×HUG, MIN/MIN; gap/padding16; no fills/effects/styles; solid #9747FF 100% stroke1 INSIDE, dash[10,5], capNONE, joinMITER, miter4; radius5/smoothing0; opacity1, PASS_THROUGH, clipsContent=true. Read back every literal chrome field; never copy another set's chrome. Direct variants retain specified sizing.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Verify the current Image default source identity and complete fill/style/reference equality for every avatar per avatar-image.md; preserve receiving geometry/provider badge. IMAGE presence alone is insufficient. Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.
