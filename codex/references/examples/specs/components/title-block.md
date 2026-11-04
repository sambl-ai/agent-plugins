# Title Block — component WHAT

WHAT for the selected reference Dashboard product-source closure.
The selected screen plan authorizes this source when it is missing. Reuse compatible sources without changing their defaults.

Use [component plan](../component-plan.md), [current context](../current-context.md),
[shared delivery](../../references/delivery.md) and [acceptance](../acceptance.md).
Build this source only when needed by the selected screen. Afterwards it is a read-only consumer contract. Dashboard Shell is a component name, not another screen.

## Goal

Create Title Block as a reusable local product source for the selected Dashboard contract.

## Target And Boundary

When a compatible source is absent, create it. Destination: the file/page explicitly named by the user's Examples request, within its `Product Components` Section. Create only this new product source; preserve existing kit sources, variables/styles/modes, assets and unrelated content. Cleanup: no existing-output cleanup. Only the exact new Slot auto-duplicate/orphan definition consolidation explicitly declared in Construction Notes is permitted; no other node, scratch or property cleanup. Declared consumer Slot-content replacement does not change kit defaults. This initial-create document does not authorize repair of existing partial output. No detachment, remote-library import, reference-page cloning or publishing.

### Target-resolution preflight

Inspect page direct children and immediate children of approved Sections. Reuse one complete compatible source unchanged after checking its contract. Create only if no exact source candidate exists. Partial, duplicate, unreadable, user-edited or incompatible candidates are real conflicts; ask for a focused disposition instead of silently adopting or replacing them. Resolve dependencies locally by exact display name/type/ancestry/API. Resolve variable path+type in its current migrated collection owner (possibly Core). No historical IDs, fuzzy matching or restored axes. If a required dependency is proved absent, follow the shared general substitution policy in delivery.md before dependent writes; do not silently change the target or repair existing sources.

## Component

Display name: `Title Block`. Two variants: Context=Standard then Context=Account. Standard default.

Set descriptionMarkdown: “Page heading and breadcrumb context, with an account identity composition.”

## Props

`Context` VARIANT Standard/Account, default Standard. Context is a structural dimension context=standard/account, not size or interaction. No Size Class or invented text properties. Page content edits existing nested Breadcrumb/ Semantic Text/Button APIs.

## Layers

- Root COMPONENT vertical FIXED × HUG, initialwidth784 literal, gap space/400; screen instances FILL width.
- Both: linked 💠 Breadcrumbs HUG × HUG first; its Items true Slot contains one native 💠 Breadcrumb Is Last=True,State=Disabled,Is Current=True,Is Focused=false. Standard label Breadcrumb; Account label My account. Replace source defaults through the supported consumer Items override with exactly one new linked current Breadcrumb; require exact local family/API/ancestry and the native Slot evidence checks below, not exposed preferred-key equality alone.
- Standard: 💠 Semantic Text Style=UI Header L,Text=Text,Has Slot Start/End=false, FILL × HUG; then 💠 Separator Direction=Horizontal,Size=100 FILL × HUG.
- Account: between Breadcrumbs and Separator insert `User` FRAME vertical FILL × HUG, cross-axis CENTER, gap space/350. Its `Avatar` FRAME horizontal HUG × HUG contains Rich Icon Size=900,Shape=Circle,Has Image=true,Has Stroke=true,Has Icon/Has Slot=false with the complete current local Image component default paint in avatar-image.md; absolute Rich Icon Size=300,Shape=Squircle,Has Stroke=true,Has Icon=true,Icon=logo_figma_color,Has Image/Has Slot=false at x55.455078125,y52.66650390625 relative to80×80 Avatar. These source-authored badge offsets are intentional literals.
- Next User child `Text Block`: vertical FILL × HUG, gap0; linked Semantic Text UI Header L Text=Bo Gydza then Compact S Text=Signed in with Figma, both FILL × HUG, no Start/End Slots; centered text alignment.
- Last User child linked 💠 Button300/Secondary/Neutral/Default,Label=Sign out,Has Label=true,Has Icon Start/End=false,Has Slot=false,Is Focused=false, HUG × HUG.

## Variant Order

Two variants: Context=Standard then Context=Account. Standard default.

## Default References

Local 💠 Breadcrumbs and 💠 Breadcrumb with its current-item API; 💠 Semantic Text UI Header L/Compact S; 💠 Separator Horizontal100; 💠 Rich Icon900/Circle and300/Squircle; 💠 Button300/Secondary/Neutral/Default; local logo_figma_color and the complete current local Image component default paint in avatar-image.md.

## Required Shared Token Rows

Reuse only the existing exact semantic paths in Size Tokens and Visual Tokens; no shared row creation. Current migrated owner/type must resolve uniquely. Preserve dependency-owned component tokens.

## Size Tokens

Bind Root gap Core FLOAT `space/400`, User gap Core `space/350`; Text Block zero-gap. Preserve kit Rich Icon native size/shape geometry and all Button/Semantic Text/Separator bindings. Avatar badge position remains declared literal; do not replace with guessed token.

## Typography

Use linked Semantic Text UI Header L and Compact S. On each existing consumer TEXT governed by its Semantic Text `Text` property, use the Typography override `textAlignHorizontal="CENTER"` for Account name/provider copy and `"LEFT"` for the Standard heading. Load current fonts; preserve copy, typography styles, color/bindings, property references, bounded width and instance links. This alignment is not inherited-frame geometry: do not resize/reparent nested frames, edit a primitive source or detach. The owned Avatar FRAME is constructed separately under Construction Notes; its inherited Rich Icon geometry stays unchanged. Reacquire the TEXT and verify alignment and visible bounds, or report the exact unsupported target/operation. No new styles.

## Visual Tokens

All owned wrappers transparent. Preserve linked semantic text/color and Rich Icon stroke/mask. Avatar uses the complete current local Image default picture/paint as the human-approved historical-avatar substitution, not a hash-only assertion. Provider logo keeps its multicolor artwork; do not recolor it as a monochrome icon.

## Interaction Tokens

None. Preserve nested kit behavior; no new motion or prototype service implementation.

## Construction Notes

### Portable Build Protocol (shared)

The complete pinned Portable Build Protocol is a mandatory separately delivered shared resource. See [delivery prerequisites](../../references/delivery.md); a link or prior-read claim is not its contents.

### Component-specific construction

Create no variables/styles. Reuse the listed exact semantic paths and preserve kit bindings. Frame defaults unless overridden: no paint/stroke/effect, zero padding/gap, NO_WRAP, MIN alignment, clipsContent=false. Instances inherit source names; owned nonzero-radius layers use smoothing0.6. Report declared fixed geometry/chrome as literals.

Both Contexts are retained by the selected full stable source API, even when this one Dashboard screen uses only Standard. Instantiate exact Breadcrumb and Rich Icon native tuples first. Account provider badge must preserve the observed composition and remain unclipped by Avatar/User. Use the user-selected current Image default picture; no historical personal photo or remote image/component dependency.

Avatar geometry: configure the owned horizontal FRAME with layoutSizingHorizontal=HUG, layoutSizingVertical=HUG and clipsContent=false. Main Rich Icon stays layoutPositioning=AUTO at its native token-bound 80×80; badge stays ABSOLUTE at native 32×32 and the declared offsets. Let layout settle, then require Avatar 80×80 with both sizing axes still HUG and the badge visibly unclipped by Avatar/User. Never compensate for a wrapper error by resizing Rich Icon, changing its dimension bindings or editing its internal Slot. Before compatible reuse, inspect this selected Account branch, not only Standard/API/version; mismatch requires separately authorized repair, never initial-create replay.

Avatar override: receive the complete [current Image default contract](../avatar-image.md). Resolve the exact current local Image component and capture its entire default fill array, paint attributes, style identity/reference and image reference. Reuse that complete current default picture/paint on this linked Rich Icon consumer Image through the supported image-fill route, preserving receiving geometry/mask/stroke and provider badge. Matching inherited state stays read-only. Verify full equality to the captured current default after writes; IMAGE presence or hash alone is insufficient. Do not use the historical personal avatar, bundled bytes, network media, invented photo/style or kit source mutation. Missing/ambiguous current Image identity or unsupported consumer application is a precise dependent gap.

Breadcrumb Items point of use: read the existing Breadcrumbs Items shared SLOT definition, preferredValues and every Slot setting, including allowPreferredValuesOnly; preserve all of them unchanged. Resolve the exact canonical local Breadcrumb family, source API and mainComponent/owning COMPONENT_SET ancestry for the required terminal tuple Is Last=True,State=Disabled,Is Current=True,Is Focused=false. Display name or localness alone is insufficient. Exposed preferred-key inequality alone neither fails this preflight nor authorizes remapping, allowlist edits, relaxed enforcement or imports. If exposed keys differ, inspect the existing nonempty source/default Items content read-only: its actual mainComponents must prove this exact local family and support the required terminal tuple, with an explicit native limitViolations=[] result. An empty Slot, absent/unreadable getter or inferred empty result is not evidence. That bounded source-content evidence permits construction using the resolved family; it does not prove internal remapping or a future consumer pass.

Create a new linked instance of the exact resolved terminal tuple, then replace this consumer's inherited default Items through the supported native consumer Slot override. Never move or clone source/default instances, mutate shared defaults, append alongside them, or park inherited virtual descendants in a hidden frame. After all property/content writes, reacquire the actual populated consumer and require exactly one current Breadcrumb with the correct tuple and context label (Breadcrumb for Standard, My account for Account), exact local mainComponent/family ancestry, unchanged strict settings/preferred metadata, and an explicit native limitViolations=[]. Any violation or missing/ambiguous evidence is a failure or gap. Earlier actual HAS_NON_PREFERRED consumer violations remain failures; a different source check does not reclassify them.

Use the shared native grouping policy: group related work within the provider budget, retaining per-group Slot lifecycle checks before dependent writes and scoped cleanup identities. Apply descriptionMarkdown to this source and its direct variants.

Use the current/latest Auto Layout supported by Figma; preserve this layout contract. No separate migration, version audit or manual Inspector gate is required. Check padding/minima, inside strokes, Fill children and effective geometry.

After combineAsVariants: vertical NO_WRAP HUG×HUG, MIN/MIN; gap/padding16; no fills/effects/styles; solid #9747FF 100% stroke1 INSIDE, dash[10,5], capNONE, joinMITER, miter4; radius5/smoothing0; opacity1, PASS_THROUGH, clipsContent=true. Read back every literal chrome field; never copy another set's chrome. Direct variants retain specified sizing.

## Stop Conditions

For an available linked Breadcrumb family, ambiguous API/ancestry, unsupported required terminal tuple, missing bounded native-valid source evidence when exposed keys differ, or a violating final consumer readback is a dependency failure/gap. A proved absent Breadcrumb instead uses the shared general substitution policy, preserving required breadcrumb meaning with honest ownership and source/Slot parity N/A. Exposed preferred-key inequality alone is not a blocker or remapping permission. Preserve the kit/allowlist; unsupported consumer Items replacement stops, with no hidden parking. Stop on target/dependency ambiguity, missing semantics or unavailable suitable dependency replacements, unresolved current axes, unavailable true Slots, orphan/duplicate Slot properties outside the exact authorized consolidation envelope, remote references, impossible tuple or required source mutation. Stop if a requested operation exceeds the approved owned-output boundary. No guessing, fake Slots, detachment or restricted-provider bypass. Proven absent dependencies may use the declared general substitution policy; report replacements, lost API and parity checks N/A.

## Page Artifacts

None. Create only this source in Product Components.

## Component-Specific Readback

Reacquire Avatar: FRAME, horizontal HUG×HUG, settled 80×80, clipsContent=false; main Rich Icon AUTO 80×80, badge ABSOLUTE 32×32 at x55.455078125/y52.66650390625. Verify unchanged child bindings/links and unclipped badge in the Account source and each selected consumer.

After all writes, reacquire the actual populated Items consumer: exactly one current Breadcrumb, required terminal tuple and context label, exact local mainComponent/family ancestry, unchanged complete Slot settings/preferred metadata and explicit native limitViolations=[]. A source-only or empty-Slot pass is not consumer proof. Verify the current Image default source identity and complete fill/style/reference equality for every avatar per avatar-image.md; preserve receiving geometry/provider badge. IMAGE presence alone is insufficient. Component checklist for the shared final check: exact identity/type/parent; declared tuples/order/defaults and visible property order; linked source/name inheritance; listed bindings/styles/literals; owned Slot settings/shared keys/true backing counts; unchanged foundation objects. Check this component's specified narrow/wide topology and settled content fit. Do not require a manual Inspector gate or collect test timings.

## Account provider badge parity correction (0.1.3)

This explicitly overrides the inherited Color surface for the Account provider badge only. Bind its existing consumer Color layer to the current local COLOR `colors/layer/floor-2` at paint opacity1, never overlay/neutral or a literal white RGB. Resolve the current collection owner by semantic path/type. Rotate the whole linked Rich Icon300/Squircle badge to Figma rotation=-5 degrees; retain its32x32 variable-bound size and declared x55.455078125/y52.66650390625. The nested logo retains local rotation0 and multicolor artwork. Preserve all stroke, mask, Slots, Avatar80x80 HUG/HUG and complete current Image paint.

Read back background alias AND opacity, whole-instance rotation AND full relativeTransform: [[cos(5deg),-sin(5deg),x],[sin(5deg),cos(5deg),y]], within floating-point tolerance. Verify the Account source and a disposable populated consumer. A correctly colored logo alone does not prove the badge background. Never rotate only the nested logo/vector. Initial-create is not repair authority; a repair uses separately authorized existing-source scope.
