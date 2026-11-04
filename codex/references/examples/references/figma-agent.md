# Native Figma Agent adapter

Use the native JavaScript writer in the user's current writable Design file.
Resolve current file/page and required local component, variable, style and asset
identities from host evidence. Keep runtime IDs local; static docs contain none.
Do not emulate the document, use REST for design mutations, install a runtime or
fetch external SVG/image assets. Use the current/latest Auto Layout supported by
Figma, preserving the specified layout; no separate version audit is needed.

Read only relevant source catalogues and owned output. Resolve semantic paths
and types in their actual current collections, including Core after migration.
In recognized Sambl mode, Core means the service role, not a display name.
Resolve one valid sambl/collection-role marker {"schemaVersion":1,"role":"core"};
legacy case-insensitive Core is allowed only after all markers were read empty.
Unread, omitted, malformed or duplicate role data blocks canonical construction.
Preserve actual IDs/names/metadata; never stamp or repair roles. Adapted mode
follows its entry policy using available resources, without requiring Sambl Core.
Keep actual breakpoint mode IDs, display names and STRING selectors separate.
Use the current Image component's complete default paint/style/reference for
declared avatars, preserving crop/transform/filter/opacity, not merely imageHash.
Native-color logos keep colors, authored geometry and rotation; recolorable icons
use their declared consumer color role. Kit sources and their Slot defaults
remain unchanged; inspect only the dependencies this output actually uses.

Keep a compact local ledger of created roots, source identities, property keys,
completed operations and warnings. A small shared owned-output manifest may
record this version and owned artifact IDs for subsequent safe reuse; it is not
an execution runtime, a scene dump or independent proof. Preserve unrelated
manifest entries and user content. Do not transmit raw scene trees to MCP.

For native Slots: create backing first, retain its automatic definition, verify
slotContentId and the prescribed full settings. Select instance tuples before
insertion; use supported consumer Slot insertion, not SLOT via setProperties.
Reacquire after changes and read actual limitViolations. Do not weaken preferred
restrictions or silently bypass an explicit provider restriction. Load actual
fonts before text writes. Matching inherited fields are assertions, not setters.

Distinguish owned nodes, inserted roots, consumer-owned content and inherited
descendants. Use settled bounds after property changes. Native Sections support
direct bound stroke width/paint, corners and smoothing: use those fields, not an
extra Surface. Apply presentation after geometry. Full-copy fit and clipping are
checks, not inferred from a scroll setting or frame dimensions.

Proceed automatically from self-checked sources to the selected screen. A native
error stops affected work with target/field/error disclosed; do not probe bypasses,
replay successful work or infer a failed operation from an untried capability.
If the host stops the request, retain partial output and report it honestly.
A credit warning is not evidence that an already running request has stopped.
No Codex receipt, manual Inspector gate or report acceptance call is needed.
