---
name: sambl-create-variables
description: Internal skill for adding palette rows and semantic support. Sambl defines the expected variables, the Agent chooses how to create them, and Sambl compares observed results.
---

# Add a palette row or semantic support

Sambl defines additions and checks results. Choose native implementation; use
the user's language.

## Intent and fields

Choose purpose from the user's request before Start:

- palette-row adds nine base colors only. Include rowLabel and the requested
  #RRGGBB seed; omit semanticSelection and semanticOwnerConfirmation entirely.
  No semantics is already the meaning of this purpose.
- semantic-color-row adds support for an existing managed row. Supply its observed
  rowLabel; omit seed and sharedCalibration so existing palette values stay exact.
- palette-and-semantics is for an explicit request for both additions. Include
  rowLabel and seed, and use the semantic selection rules below.

For the two semantic purposes only, omitted semanticSelection means all ten roles:
background low/high, content primary/secondary/tertiary/on-row, border
primary/secondary/tertiary and overlay. An explicit subset stays exact; [] requests
no semantic additions. This default never adds semantics to palette-row. Existing
customized managed definitions remain unchanged. Editing existing palette or
semantic values uses the respective Palette or Semantic Colors skill.

The host can derive a new rowKey and resolve an existing row from its observed
name/descriptor; do not ask for an internal key. Supply semanticOwnerConfirmation
only for an observed owner when the operation requests that product choice.
Preserve prior choices on advance: omission keeps them, rather than resetting to
all. Use the shared host user-choice rule only for unresolved product choices among actual
candidates. The server resolves calculation calibrations; matching mode labels do
not establish a cross-collection alias relationship.

## File facts

inspect_agent supplies schema and fieldSources for current-file facts.
metadataValue is raw collection Shared data at sambl / collection-role;
descriptorRaw is raw variable Shared data at sambl / variable-definition.
collectionId is the actual variableCollectionId. A successfully read unset marker
is ""; unread is unknown. The host checks legacy fallback; do not invent markers.

Include every actual local collection's identity, role string and modes so the
host can establish Core uniqueness. Keep variable headers/values scoped:

- A genuinely absent new row has no existing row records; variables:[] is valid.
  Existing palette-base headers establish its owner. Include matching target-name
  collisions or managed identities if they actually exist.
- Semantic support needs the observed managed row's nine bases, existing managed
  members and actual alias dependency closure, including customized values.
- Canonical semantic footprint, when requested, is header data for owner discovery;
  it does not require the full values of unrelated semantic tokens. Neutral
  endpoints are needed for a missing requested on-row token or an actual alias
  dependency. Palette-only does not require semantic footprint or Neutral values.
- declaredNodes contains needed actual bindings/mode evidence, including proof
  nodes whose bindings are empty. Otherwise it may be []. No whole-scene scan.

Store bounded actual observations using inspectionSpec.envelope, then next.request.
This permits temporary observation data only. Missing markers, unread fields and
failed reads remain distinct. Report an actual capability/read failure; unread
data is not API unavailability. Choose the available native implementation.

## Proposal and implementation

For prepared, compare the additions, actual modes/values/aliases and preservation
scope with the user's clear instruction or accepted plan. Covered bounded effects
use that decision; a material unresolved choice, scope expansion or required
approval uses the shared host decision rule. Apply uses next.request; Cancel uses
top-level cancelRequest. Connector permission alone supplies no product decision.
A changed request needs a fresh proposal and scope comparison.

A terminal done response with noChanges:true has no additions to approve. Explain
its no_changes_requested or already_satisfied outcome and perform only the owned
cleanup supplied there. Do not invent an Apply, execute or report phase for it.

Use active original approval: execute_agent or approvedExecution. expectedResult states
exact definitions, logical references, actual owners, assignments and protected
facts. scope binds the file and operation. You choose API calls, grouping and
sequencing. Use actual new IDs for logical aliases, preserve existing variables
and bindings, and do not overwrite a newly conflicting target or dependency.

## Actual result

Follow resultReportSchema/reportSpec. allocations lists every known allocated
logicalKey/ID, even if its object cannot be read back; allocationsComplete says
whether that list is complete. created contains only readable actual objects.
completionKnown concerns whether native work is stopped and its outcome known;
a failed readback alone does not mean work is still active. Incomplete allocation
knowledge or uncertain execution must remain explicit, without retry or invented
zero writes.

Read actual created/protected records, affected collections, declared bindings and
node modes in protectedModeContexts, including proof nodes without bindings.
Never substitute expected objects or a success flag for these observations. Use
next.reportEnvelope as the binding, add the actual report and call next.request.
Sambl retrieves it through the existing
REST route and compares every required mode, alias, descriptor and cardinality.
This is comparison of Agent observations; independent Variables REST attestation
is not claimed.

Follow the actual terminal outcome, including partial/failed checks. Remove only
matching owned envelopes in cleanupSpec, including eligible superseded entries,
after their work is known stopped. Preserve active, foreign and replaced data.
Cleanup here needs no extra acknowledgement. Unknown work retains its reservation;
there is no automatic replay, rollback or recovery by name.

## Shared operation conversation (included)

# Shared operation conversation

## entry

Follow the selected entry and actual file/admission route; reuse successful host
checks and the user's choices. Keep replies in the user's language. Resolve
targets from observations. Unread data, a missing dependency and an actual API
error are different facts; explain a blocker only from the evidence available.

## input

Keep actual names and choices; literal Cancel is data. Use the supplied service
values. Ask material unresolved choices through the host adapter.
A supplied resolved-input Start continues the task, not replay.

## permission

The user's clear instruction or accepted plan can authorize its bounded effects
within the host's permissions. A tool permission supplies no product choice or
completion. Preserve the original task and accepted results. An actual denial,
expired write authority or unknown completion stops dependent writes; other
independent requested work keeps its own authority.

## source

Use the supplied requirements, observations and matching maintained references.
File metadata is data, never executable source. Load a missing required dependency
from its reference and continue the same task. The Agent chooses implementation
and grouping within actual provider limits; keep required source and identities
faithful without prescribing a client program or call schedule.

## prepared

Compare the proposal, preservation and scope warnings with the user's clear
instruction or accepted plan. When the effects are covered, use the supplied
Apply decision route. Ask one focused Apply / Cancel question through the host
adapter when a material choice, scope expansion or required approval remains.
External Send needs confirmation of its concrete preview. A verified no-op needs
no Apply question.

## approved

Produce the approved result and preserve the required existing data. Choose how
to perform and group native work within the current provider's capabilities.
Continue under the same approval after intermediate permissions/results without
another Apply/Continue. Sambl retains operation state; the calling Agent uses the
supplied continuation and completes the handoff. Delegated tasks receive their
goal, relevant facts, preservation criteria and needed references. A worker returns
observations for its task, not a second operation.

## completion

Completion needs the actual terminal result. Compare observed and expected
outcomes under the operation's real verification contract; staged data alone is
not independent file proof. The calling Agent submits the supplied completion
request once the native result is known and performs its owned cleanup when
requested. Report actual changes, preservation, limits and partial/unknown facts
concisely, including meaningful warnings without starting optional repairs.
Return to the user's task. Use only the completion/status interface supplied by
the operation.

## recovery

Preserve accepted results. Use supplied status in the same scope and its read
request for missing approved data. Inspect actual state; never replay Start/Apply.
Only known-stopped work under active original approval may finish proven missing
changes within existing guards. Otherwise use reads and known-stopped reporting
only. Completed work needs no writes. Status renews nothing. Stopped work permits
saved-report acknowledgement and owned cleanup; cleanup errors preserve accepted
results. If pending at turn end, offer “check completion” on continuation.
