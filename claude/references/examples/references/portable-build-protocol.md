# Portable Build Protocol

### Complete context before writes

Resolve required immutable reference/versions once and retain their complete
contents. The executor, including a delegated child, needs this protocol, selected
complete WHAT, content/media and authorized context: destination, current axes,
dependency identities, owned output and cleanup scope. Forward successful
contents rather than refetching; a parent summary/key/version is not that payload.

Retry failed/truncated delivery within its bound, retaining expectedVersion and
checking returned Resource URIs. Missing complete context stops dependent writes.
Version mismatch uses the entry's fresh-package recovery; preserve choices and
completed output instead of unpinning or replaying construction. A requested
additive build needs no redundant approval; replacement or broader mutation needs
its own authority. No whole-file census is required.

### Selected scope and shared reuse

For page/screen generation, each invocation covers one explicitly selected
page/screen, its required current modes and dependency closure. Ask when the
selection is missing; never infer all pages from an available catalogue. Before
executing missing dependencies' initial-create inputs, verify and reuse compatible
owned shared components unchanged: prove ownership and compare actual identity,
API, bindings, structure, supported behavior and settled state with the current
relevant contract. Delivery packageVersion pins one coherent instruction load;
it is not an artifact compatibility version. A global package hash changing due
to another document or Community data is not itself a source conflict. No old
package is needed or retained. A local provenance note is a discovery aid, not
proof of compatibility or permission to overwrite. Reuse skips that source's
create input; it does not relax the initial-create zero-candidate guard. Missing
sources still require that guard. Preserve user edits and unknown ownership;
partial, ambiguous or actually incompatible output needs a focused disposition.
Do not edit or recreate existing shared families or prior screens to accommodate
the next page. Verify the selected variant's settled geometry/content, not only
family API or a recorded version.

Perform one affected-scope check, report only that selection's completion/gaps,
then invite the user to view the result. Scoped acceptance is not whole-catalogue acceptance.
Propose the next page separately and obtain user agreement before its invocation;
do not automatically continue or build the remaining catalogue in bulk.

### Reuse across retained breakpoints

Resolve sources, styling, content and actual modes once while fresh. Reuse common
content construction across all retained breakpoint outputs, applying their exact
shell tuples and layout differences: Dashboard md/lg GRID, sm/xl HORIZONTAL+WRAP.
Mode switching alone does not supply those differences.

Whole owned-instance duplication needs prior proof on that provider of source
links, true Slots/backlinks, content, overrides and bindings. For the current
unproved populated-Slot route use fresh exact source instances and common content
construction; do not run clone experiments during generation. Direct Slot cloning
returns a Frame. Existing source/consumer lifecycle rules below still apply.

Group related native work by actual runtime/payload budget, not fixed operation
counts. Verify Slot lifecycle groups before dependent writes and keep scoped
cleanup identities. Reuse valid facts and loaded fonts; native handles do not
persist between calls. Let shared-source changes settle before reading dependent
instances. Combine affected-scope readback and visual review.

### Dependency roles and strict identity

Distinguish a semantic role (such as trailing navigation affordance) from a
contract requiring an exact component, variant or asset. Resolve a role through
the current local primitive's public API within the dependency scope;
do not guess a glyph from its display name. Strict identities remain strict.
Read actual prop types/options, native tuple, Slot definitions and supported
content before inserting. Names/appearance do not prove compatibility or identity.
Missing/ambiguous API returns a bounded gap.

For every restricted Slot read the current shared definition, `preferredValues`
and `slotSettings.allowPreferredValuesOnly`. Resolve the exact canonical local
family through its public API, actual `mainComponent` and required owning
`COMPONENT_SET` ancestry. Names, localness or appearance alone are insufficient.
Distinguish that identity from equality of exposed preferred-key strings. Key
inequality alone is neither an automatic identity failure nor permission to remap
preferred values; do not infer an internal remapping mechanism from it.

Where exposed keys differ, require bounded read-only evidence of nonempty,
native-valid source/default content linked to that same exact local family,
together with the current Slot definition/settings and an explicitly readable
native `limitViolations=[]`. An empty Slot, missing getter/field, unobserved value
or ambiguous family is not this evidence. Missing evidence remains a gap; do not
create scratch content or a new test framework to manufacture it.

During already-authorized construction use only the resolved native family/tuple
and supported consumer-content replacement. After all property writes, reacquire
the actual populated consumer and verify intended content/count/tuple, local
main-component ancestry, unchanged Slot settings and preferred metadata, and
explicit native `limitViolations=[]`. A source pass does not prove a future
consumer pass. `HAS_NON_PREFERRED` or any other violation fails that consumer;
previous observed violations remain failures, and missing readback remains a gap.
Advisory preferences and enforced restrictions are different. Never edit source
defaults, allowlists or Slot settings to resolve a mismatch, import dependencies,
loosen restrictions or substitute a lookalike to pass.

### Native Slot source lifecycle

For a new standalone source, create the native Slot and reuse its auto-created
`SLOT` property; never pre-add a second same-name property.
Read the exact definition key and backing `componentPropertyReferences.slotContentId`;
require one public definition per role and the contract's backing count.

For an explicitly permitted new ComponentSet, combine fresh empty variants. The
first native Slot establishes the retained shared key. For each further variant,
create its native Slot, record the exact auto-created duplicate key/backlink, and
confirm the backing still reads `SLOT`. Only under the run's pre-authorized
consolidation envelope, remove that exact newly created duplicate definition,
assign the backing's `slotContentId` to the retained key, then reacquire and prove
one shared definition, every expected true backing and no orphan. Do not batch
past a failed group. Never delete the retained shared key or an existing source
property. Do not clone Slot-bearing sources: a cloned backing can become `FRAME`.
Unexpected conversion, missing backlink or count drift stops construction.

### Consumer content and hidden Slots

Instantiate the exact native dependency tuple before filling its true Slot. Do
not swap or clone a populated Slot-bearing dependency across axes. Reacquire from
a stable retained ancestor after property writes; old virtual handles may be
invalid. Append content to the true Slot node, never set a `SLOT` value through
`setProperties` or use a plain Frame as a fake Slot.

Declare source defaults and consumer behavior: retain, replace or append. For
replacement, materialize the owned consumer's Slot content using the
supported native route and replace only that consumer override. Never move source
or inherited virtual descendants into another parent, mutate shared defaults,
park them in a hidden Frame, or broadly reset an instance. If native replacement
cannot be performed within the declared ownership, stop with the exact gap.

For hidden Slot access, save `figma.skipInvisibleInstanceChildren`, set it false,
reacquire the real ancestor/Slot, then restore the flag in a finally path. Preserve
document visibility. If unsupported, only a recipe-authorized temporary Boolean
reveal is allowed; restore values/backlinks and reacquire. An empty traversal is
not proof that the Slot or its contents are absent.

### Host-aware geometry

Classify target/field: owned source/wrapper, primary insertion root, consumer-owned
Slot content or inherited instance descendant. Matching inherited fields: read-only;
TEXT paragraph formatting is not layer geometry. Source-build prose permits no consumer-descendant writes; nested nodes are not universally immutable.
Parent type/layout/lock proves no write capability. Preserve links/allowed overrides;
never edit primitives, detach or add forbidden wrappers.

Source AND recipe must permit true consumer Slot itemSpacing binding: it affects
layout but sets no x/y, width/height, rotation, constraints
or axis alignment. Resolve Slot/backlink/local token; retain defaults/settings and
other inherited fields. No other geometry/source edits.
Use provider-supported routes; explicit restrictions stop without probing. Other-field restrictions imply no itemSpacing ban. Report target/field and restriction or call/error; untested is unverified, not runtime failure.

Inspect host type/layout/sizing/constraints/bounds. FILL needs parent support;
layoutMode=NONE Slots/absolute hosts may need fixed child sizes/constraints.
Never convert hosts to auto-layout or override primitive contracts for FILL.
Retain dimension bindings/aspect ratios.

Measure settled host bounds before child fitting and after resize/property writes
or permitted clones. Ignore stale source/initial sizes. Only full-host contracts use local x=0/y=0, resolved host width/height and supported edge
constraints. Read back after layout: local coordinates, effective bounds, required
descendants, clipping, full scrim/viewport coverage, not just root/size.
Centered/inset content need not use zero origin.

For full text, use a documented consumer Typography override on existing
TEXT: load current fonts; retain copy/styles/colors/bindings and bounded width.
Set textTruncation="DISABLED", maxLines=null with height-growing sizing. No invented
Wrap props, auto-layout wrapping changes, primitive edits or global truncation
disable. Reacquire/verify full text/ancestor bounds; unsupported routes remain gaps.

### Exact cleanup authority

Before creating scratch nodes or consolidating Slot definitions, the run must
authorize cleanup of those new objects and declare their parent scopes, roles,
expected counts and backlink outcomes. Record exact ids/definition keys as they
are created. Before removal verify ownership, current ancestry and backlink
inventory; afterward verify expected retained counts/links. A disposable root's
removal does not prove its Slot definitions disappeared. Remove only its proven
new orphan definition under that same envelope; never an in-use shared key.
No recursive name/prefix deletion, hidden parking, existing-user cleanup or
retroactive authorization. Unknown prior partial residue needs a new decision.

### Current axes and media

Use only verified current collections/modes/selectors and the recipe's structural
mapping. Keep labels, selector values and composition baselines distinct. An
absent axis and present singleton are different; neither permits restoring old
modes or duplicating unused variants. Inherit the retained environment.

Media instructions distinguish required delivered assets from an explicitly
approved existing kit Image placeholder. A placeholder route preserves the
resolved Image source and its complete image paint: image reference, scale mode,
transform/crop, filters, opacity and other present fields, plus applicable style
identity. Do not copy only an image hash or download a replacement. Missing a
required asset is not automatic placeholder permission. Do not invent a new
placeholder style. Verify complete paint/source equality or report it unproved.

### Interruption and final result

Keep a compact local ledger of this actual file/request, current instruction
pins/configuration, exact owned ids, completed operations and unresolved gaps.
This is local working context, not a server receipt or a new permission token.
On resume, check the actual same target and relevant state before reusing owned
work, preserve intervening user edits and ask only on a real conflict or changed
scope. A saved success claim or ledger entry alone is not current evidence.
Refresh instructions through the entry if their pinned delivery is unavailable;
do not replay construction merely to correct a final message.

Perform one final check of owned output and declared protected controls. Show the
user a concise result, actual screen/component links when available, and an
invitation to inspect the result. Keep scratch ids and diagnostics in the local
ledger, not the user-facing result. State actual substitutions, omitted content,
unchecked fields and failed requirements without hiding defects. A compatible
substitution can complete with a warning; missing required geometry/content,
invalid preferred content or unverified required media cannot be called finished.
Changing the message cannot change the actual outcome. API readback alone does
not prove visual or interactive correctness; identify remaining limitations.
No final MCP report, server validation callback or mandatory acceptance turn is
part of Examples.
