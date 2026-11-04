# Nav Bar — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Nav Bar as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Nav Bar`. None. One COMPONENT.

Set descriptionMarkdown: “Compact product navigation bar with menu control and Sambl identity.”

## Props

None. No Size Class property. Configure the linked kit regions through their existing APIs; do not add product wrapper controls.

## Layers

- Root COMPONENT vertical FIXED × HUG, initialwidth375 literal, minWidth bound to main-layout width selector, inline padding space/350, block padding space/250.64px observed settled height is not a fixed Root rule.
- One linked kit 💠 Nav Bar, FILL width × FIXED44 height; preserve its existing components/nav-bar/size/base/root/min-height binding and gap. Has Start/Center/End=true; all three regional helpers use Custom.
- Start true Custom Slot contains exactly one linked 💠 Button300/Secondary/Neutral/Default,Has Label=false,Has Icon Start=true,Icon Start=exact local menu,Has Icon End=false,Has Slot=false,Is Focused=false.
- Center true Custom Slot contains exact local logo_sambl-full_color with governing height size/150 and preserved aspect ratio.
- End true Custom Slot contains exactly one ordinary owned FRAME named Empty, FIXED48×32, layoutMode=NONE, transparent, no strokes/effects/children, no dimension bindings. It is legitimate reference product-owned content, not a helper Empty variant, Service Layer or fake Slot. Keep Has End=true.

## Variant Order

None. One COMPONENT.

## Default References

Local kit standalone 💠 Nav Bar and 💠 Nav Bar Start/Center/End with Custom true Slots; 💠 Button exact300/Secondary/Neutral/Default; local menu and logo_sambl-full_color.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Root minWidth binds existing FLOAT shared-components/main-layout/size/base/root/width; inline padding space/350; block padding space/250. Preserve kit gap and min-height bindings. Menu Button icon geometry retains components/button/size/300/icon/size; logo governing height uses size/150.

Inner kit bar height44 and End Empty width48/height32 preserve the observed reference product-specific fixed representation. They are explicit intentional literals under this WHAT; retain the existing min-height binding and do not replace any of them with a numerically matching token without purpose/type/mode equivalence. Record node/field/value/reason. Create no variables or styles.

## Typography

None. Label is hidden; no new styles.

## Visual Tokens

Root transparent. Bind swapped menu consumer Vector to existing COLOR `components/button/variants/variant/secondary/intent/neutral/layers/content/color`; do not repaint atomic source. Preserve logo multicolor artwork.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Instantiate each exact Custom helper before filling its actual native Slot. Matching inherited representation is a read-only assertion. The fixed44 primary kit-instance insertion-root size and new End Empty Frame are explicitly scoped product-instance/content overrides; never edit kit masters or inherited helper geometry/settings/defaults. Use only a supported route; an actual restriction is a precise dependent gap, never a bypass. Retain inherited instance names/exposure and all Slot settings/preferred metadata. Do not use old parent Variant/Slot Start/Slot Center/Slot End APIs. Reacquire and prove all native Slots valid, fixed44 bar, true End Slot with one48×32 Empty Frame and content-driven product Root.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.
