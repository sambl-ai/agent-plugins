---
name: sambl-collections
description: Keep the modes a product needs in an existing non-Core collection and adapt its related component variants and instances. Use the specialized entries for Themes, Platforms or Breakpoints.
---

# Configure a collection

Use the included Collections knowledge for the actual file and requested
collection. Resolve an explicit name from the current collections; when the target
is unspecified, offer the actual non-Core choices. Core is the shared destination,
not another axis to configure.

Reuse the user's retained modes. Otherwise ask which existing modes the product
needs, allowing one, several, all or leaving the current settings alone. Ask only
what is unresolved; names and IDs are resolved from the file.

One retained mode collapses the source into Core except `name` and removes its
matching component switch. Several keep the collection with the retained options.
Preserve other axes, instances, content and overrides under the shared outcome.
Choose the native approach; finish this task or return its actual result to the
current onboarding plan. A specific standard axis may use sambl/themes,
sambl/platforms or sambl/size-class for its product labels and presets.

## Shared Collections knowledge (included)

# Collections knowledge

Themes, Platforms, Breakpoints and other mode collections share these outcomes.
Choose native methods, grouping and useful self-checks for the actual task in the
user's current Figma copy.

## Actual file and choices

Resolve collection and mode names from the file; preserve their spelling. A unique
case-insensitive match may resolve a standard label. Similar words or variable
types do not establish a role. Clarify duplicate, missing or conflicting names only when the target is
undecided, using names rather than asking for internal IDs. An absent collection does not establish its previous selection
and need not be recreated.

Root metadata/version alone neither proves the result nor blocks a clear
structural task. Core is the shared destination, resolved only when migration or a
real dependency needs it; subset/no-op needs no Core gate. A collection-owned SharedPluginData marker `sambl` / `collection-role` with
value `{"schemaVersion":1,"role":"core"}` can identify renamed Core; preserve
it unchanged. Otherwise a unique local Core name (case-insensitive) is useful. A missing or ambiguous required destination needs
resolution, not guessing from its variables.

Keep current settings leaves the structure alone. Selecting all actual modes is
different: two or more may already satisfy the request, while configuring a
singleton still collapses it. Zero selected modes leaves the choice unresolved.
Use current facts for an unchanged result, not a historical completion marker.

## Several retained modes

Keep the collection, retained mode/variable identities, values, aliases and
metadata. Retire unwanted modes and matching component options, adapting their
actual affected assignments and instances to retained choices. Preserve the
existing default when retained. If it is removed, use a valid retained default
and tell the user which one remains. This needs no separate default-only question
or column reordering.

Reuse supplied replacement choices. Ask once for needed mappings only when real
affected uses have several unresolved retained destinations. No affected uses
means no fallback question. Mode order, pixel widths or the default do not choose
that mapping for the user.

## One retained mode

The source disappears even if already singleton or empty. Preserve every source
variable's type, selected-mode value and metadata in Core, except the service variable
named exactly `name`. No other variable is discarded because it looks internal
or unused. Migration creates new variable IDs: working references follow their
actual replacements. Keep aliases to surviving collections and redirect aliases
among migrated variables, rather than flattening them all to resolved literals.

Do not copy `name` into Core. Uses removed with the retired component property
can disappear with it; surviving uses receive the chosen literal or an equivalent
valid local binding without a new Core `name`. A real Core collision needs a
resolution that preserves intent, not silent overwriting or loss of a distinct
variable.

Relevant consumers can include aliases, node/style bindings, explicit modes,
component properties/instances and existing prototype uses. The optional
get_variable_usage_index can help find consumers; native reads cover fields it
lacks. Follow actual dependencies so removed variables, modes and collection
leave no dangling references. Removing the source must not strand consumers.
Remote sources and other files' published subscribers are outside local-copy
adaptation; resolve an encountered external dependency as an actual scope issue.

Surviving fields keep their variable relationships to the replacements, including
width, height and min/max constraints on source components and instances. The
selected mode may change a numeric size; the same number stored as a literal is
not the same binding. Keep those links through related layout and instance updates.
Resolve a missing replacement before binding: native `setBoundVariable(field, null)`
removes the link.
Useful self-checks compare surviving field links with their intended replacements;
a scan finding no old IDs cannot detect a binding that disappeared altogether.

## Components and instances

A matching variant property corresponds to the collection's actual name and mode
names, confirmed by component structure. A similar label does not bring another
axis into scope.

Cover every matching family, including one whose collection axis is its last
axis. Keep discovery compact with relevant fields; complete any partial list of
matching results rather than treating its first entries as the whole scope.

For several modes, keep existing retained branches and remove retired options.
For one mode, its branch survives for **every combination of the other axes**,
and that collection's axis and switching property disappear. The result remains a
functioning component without the switch, even if it was the last variant axis.
The native representation is the agent's choice; a one-value switch is not its
removal.

Keep existing product and example instances functioning with their other axes,
content, Slots, settings and applicable overrides. Move retired-variant instances
to the chosen retained branch; deleting or detaching instances is not a shortcut.
A missing branch or unpreservable override is a concrete conflict to resolve,
not a hypothetical questionnaire for every user.

Later Slots/Examples work uses surviving properties and actual targets. An old
pinned Slot index does not prove a changed backing/set still resolves. Reassess
such helpers within their own task; their compatibility is not a prerequisite
for this collection change. Preserve the actual Slot content and settings.

## Finish the user's task

Reuse fresh facts and resolved choices; expand reads when actual dependencies
or changed state need them. A clear bounded instruction can supply the decision
within host permissions. Ask for unresolved material choices, expanded effects
or required host approval; no separate Apply ceremony or mandatory full-file
postflight is introduced.

Explain actual retained choices and meaningful consequences in the user's
language. Distinguish changed, already matching, kept, absent and unfinished
work; the requesting task uses that same-file result. Partial or unknown work stays so.
Connection loss is not permission to repeat a completed or possibly active
migration/deletion; an active old operation needs safe reconciliation.

## API facts that affect the result

`variableCollectionId` is read-only; an existing variable object cannot move
between collections. Collection removal also deletes its variables.
`defaultModeId` is read-only. `deleteComponentProperty` does not support VARIANT.
`swapComponent` offers heuristic override preservation; direct `mainComponent`
assignment clears overrides. Choose the method for the actual content, Slots,
settings and overrides that must survive. Structural changes may invalidate
descendant handles; reacquire current descendants from a surviving ancestor.

Official references: [Variable](https://developers.figma.com/docs/plugins/api/Variable/),
[VariableCollection](https://developers.figma.com/docs/plugins/api/VariableCollection/),
[ComponentSetNode](https://developers.figma.com/docs/plugins/api/ComponentSetNode/),
[InstanceNode](https://developers.figma.com/docs/plugins/api/InstanceNode/).

## Delivered collection data

```json
{"otherCollections":{"capability":"other_collections","question":{"en":"Which {collection} setup fits your product?","ru":"Как настроить {collection} для вашего продукта?"},"presets":[{"key":"single","label":{"en":"Single mode","ru":"Один режим"},"selection":"single"},{"key":"custom","label":{"en":"Custom","ru":"Свой вариант"},"selection":"multiple"},{"key":"keep","label":{"en":"Keep current settings","ru":"Оставить текущие настройки"},"selection":"keep"}]}}
```
