# Dashboard Shell — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Dashboard Shell as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: Dashboard Shell. This source component alone does not create the Dashboard example screen.

Set descriptionMarkdown: “Responsive signed-in shell with navigation, main content and overlays.”

Exact reference source direct-child/API option order is xl,lg,md,sm, defaultxl. Screen row order follows actual collection modes; source API order and file mode order are distinct. Represent only retained actual selectors. If xl is absent, use the largest retained known baseline as default, as defined in current-context.md, preserving retained source option order. Ask only when an actual custom selector has no clear composition mapping; never invent or restore a mode. An absent axis produces one COMPONENT with no Size Class using its resolved existing geometry/baseline.

## Props

Ordered stable API: Size Class VARIANT only when the collection exists, options/default as explicitly mapped above; Is Navigation Open BOOLEAN=false; Has Overlay BOOLEAN=false; Main,Navigation,Overlay true SLOTs. Booleans/Slots are non-selectors. Navigation visibility follows Is Navigation Open on compact and remains visible on wide; Overlay visibility follows Has Overlay. Main/Overlay default empty. Every source Navigation Slot contains one linked local Navigation, including hidden compact defaults. No synthetic Size Class for an absent axis. Retain this explicit public property order: Size Class (when present), Is Navigation Open, Has Overlay, Main, Navigation, Overlay. Historical API key enumeration alone is not Inspector proof.

## Layers

- Root: horizontal COMPONENT, FIXED width × HUG height, zero gap/padding, primaryAxisAlignItems=MIN, counterAxisAlignItems=MIN, NO_WRAP, clipsContent=true, overflowDirection=NONE; viewport width/minWidth/maxWidth/minHeight bindings below.
- `Navigation`: true SLOT, VERTICAL, primaryAxisAlignItems=MIN, counterAxisAlignItems=MIN, NO_WRAP, fixedwidth256 literal, FILL height, viewport minHeight. Contains exactly one linked local Navigation FILL × FILL in ALL source variants, including hidden compact defaults. Inline/bottom padding space/350. Compact top space/450, visibility Is Navigation Open; wide top space/700, always visible. Wide consumers retain and configure the existing linked Navigation through supported consumer content overrides, including its Menu; do not insert a second Navigation. After assembly require exactly one linked Navigation in this Slot. Compact Dashboard consumers keep inherited Navigation populated but hidden, Is Navigation Open=false. Preserve source defaults; only supported consumer content overrides customize selection.
- `Main`: vertical FRAME FILL × HUG, viewport minHeight, floor-1 fill. Compact minWidth bound to shared main-layout width selector (not min-width); wide has no Main minWidth. primaryAxisAlignItems=MIN in every baseline; counterAxisAlignItems=MIN at sm and CENTER at md/lg/xl. NO_WRAP, zero gap/padding, clipsContent=false.
- Compact only: product Nav Bar instance first in Main, FILL × HUG.
- `Main` true SLOT inside Main frame, VERTICAL, primaryAxisAlignItems=MIN, counterAxisAlignItems=MIN, NO_WRAP, clipsContent=false, overflowDirection=VERTICAL at sm and NONE at md/lg/xl, FILL × HUG, maxWidth800 literal, gap space/650, inline margin selector. Compact paddingTop space/400,paddingBottom space/550; wide space/750,space/900. sm alone minWidth uses shared main-layout width; others none. Empty default.
- `Overlay`: true SLOT, absolute, pinned0 to all four Root edges, layoutMode=NONE, overflowDirection=VERTICAL at sm and NONE at md/lg/xl, transparent/nonclipping, visibility Has Overlay, empty default. It stretches without changing normal-flow height. Preserve full-host overlay geometry in the stable source API. This Dashboard state leaves Overlay empty/hidden and constructs no Popup or other screen.

## Variant Order

Reference recognized selector order xl,lg,md,sm, defaultxl. Only current retained selectors may be present; if xl is absent use the largest retained known baseline; ask only for unfamiliar selectors whose composition mapping cannot be resolved. Never copy unavailable modes from the reference. Present singleton retains its actual mapped axis; absent axis means one COMPONENT without Size Class. Source option/direct-child/default and screen row order are checked separately.

## Default References

Local product Nav Bar for compact anatomy; local product Navigation with its Menu/Menu Group/Menu Item/Account Item closure as source Navigation content in every retained source variant. Main and Overlay are empty. Exact local current semantic variables; never import reference sources or variables.

## Required Shared Token Rows

Reuse the exact existing semantic paths in Size Tokens and Visual Tokens. Resolve current owner/type and verified selector mapping; no new shared rows. Navigation source closure is required before Shell even when compact content is hidden. Main Layout remains a kit token/primitive dependency, not a new product family.

## Size Tokens

All existing FLOAT selectors under `shared-components/main-layout/size/base/root/`: Root width→`width`, minWidth→`min-width`, maxWidth→`max-width`, minHeight→`height`; Navigation/Main-frame minHeight→`height`; Main-slot inline padding→`margin-horizontal`. Compact Main-frame minWidth and sm Main-slot minWidth→`width`. Other Core FLOATs: Navigation inline/bottom `space/350`, compacttop `space/450`, widetop `space/700`; Main gap `space/650`, compacttop/bottom `space/400`,`space/550`, widetop/bottom `space/750`,`space/900`. Preserve maxWidth800 and Navigationwidth256 as product geometry literals.

## Typography

None. Linked dependencies and screen Slot content own typography.

## Visual Tokens

Bind Root COLOR fill `colors/layer/floor-0`; Main frame `colors/layer/floor-1`; other wrappers transparent.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, primaryAxisAlignItems=MIN, counterAxisAlignItems=MIN, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Known composition mapping: sm/md compact; lg/xl wide. Never hardcode four variants. At absent axis, marker/actual Core selector selects one composition. For unfamiliar modes require an explicit verified baseline/source API/default disposition in the supplied context; predecessor inheritance is permitted only when that mapping is expressly supplied, with each mode's own geometry. Source component samples inherited wrong sm widths even in wide variants: create explicit exact current size mode on each new responsive source and bind instance Size Class only when that axis exists, using the exact current STRING selector resolved by the verified adaptation/mode plan: the canonical path when present, or its verified exact migrated path when applicable. Confirm current collection ownership and supported selector values; never infer a name leaf or use fuzzy/suffix matching. A collapsed run omits that binding/property entirely. Do not populate a Slot and then switch its native owner variant. This selected Dashboard screen remains content-HUG; no other page or Popup recipe is active.

Reference-specific defaults: populate each new source Navigation Slot with one linked Navigation FILL × FILL and its linked Menu Fill-height content. Configure the navigation names, icons and item states in this Dashboard Shell source itself using the exact selected preset in content.md: an untitled first group with Connections/sparkle and Support/question-mark; a Projects group with Coming soon.../folder-open. Preserve the generic Menu Group, Menu and Navigation sources; these are supported nested instance/Slot-content overrides owned by Shell. All retained Shell variants, including hidden compact Navigation backings, carry the same complete navigation preset. No Group/Menu Item/plus placeholders may remain in those prescribed roles. The selected screen may override its selected destination through supported consumer properties; preserve unrelated local consumer overrides. Footer/current Image remain the actual existing defaults, without a separate footer/media change. Main/Overlay remain empty. This constructs a new authorized product source, not permission to repair an existing one. Compact sources/consumers keep that content hidden and closed; no extra open-navigation screen. Do not apply the later empty-Navigation/profile-pruning specialization.

Owned Slot settings for Main, Navigation and Overlay: displayEmptyByDefault=true, stretchChildOnInsert=false, null child limits; preserve declared preferred content and descriptions. Dashboard Slot creation: when the collection is present, combine only the fresh empty variants first. For each role Main, Navigation and Overlay, create the first native backing to establish its retained shared key; on each later variant create one backing, record its exact newly auto-created duplicate key and owner/backlink, and prove that backing is SLOT. Within this new Dashboard set only, remove that recorded duplicate definition then immediately assign its backing's componentPropertyReferences.slotContentId to the retained key, reacquire, and prove one shared definition plus all expected true backings before continuing. Maximum duplicate removals are one per later backing creation, 3 × (N − 1) total; never delete a retained key or existing property. After all groups require three shared SLOT definitions and N backings per role, then apply visibility/default settings. For absent collection, create three native Slots in the single new component and reuse their auto-created definitions without consolidation. For this new owner only, cleanup may also remove at most one proven new orphan SLOT definition per create operation: record its exact definition key, owner id/name/type/ancestry and role at creation; before deletion prove zero backlinks and the retained intended shared key/backings. Preserve every pre-existing definition; unknown residue or another orphan stops. This does not authorize scratch-node deletion.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

After combineAsVariants: vertical NO_WRAP HUG×HUG, MIN/MIN; gap/padding16; no fills/effects/styles; solid #9747FF 100% stroke1 INSIDE, dash[10,5], capNONE, joinMITER, miter4; radius5/smoothing0; opacity1, PASS_THROUGH, clipsContent=true. Read back every literal chrome field; never copy another set's chrome. Direct variants retain specified sizing.

## Stop Conditions

Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Verify every source Navigation backing has exactly one linked local Navigation, including hidden compact backings; check the complete content.md navigation preset in every backing and matching-scale Default typography on every group title. Generic Menu/Navigation defaults remain generic; screen-owned selected destination and unrelated consumer overrides remain supported. Main/Overlay are empty. Confirm Menu fills Navigation and all native Slots have explicit limitViolations=[]. Check exact retained source API option/direct-child/default policy separately from actual file mode and screen row order. Component checklist: exact identity/type/parent, declared props/tuples/order/defaults, links/names, bindings/styles/literals, settings/preferences/backlinks/true backing counts and unchanged foundations. Check declared property order and updated layout. Use a screenshot where supported; API enumeration alone does not establish visual correctness. No manual Inspector acceptance turn is required.
