---
name: sambl-onboarding
description: Guide general Sambl setup and preparation of a supported Sambl UI Kit copy. Use direct child workflows for a specific task and get_capabilities for general capability questions.
---

# Sambl onboarding

Own the onboarding conversation and local progress. Use each child's actual
result; operation completion belongs only to children that use an operation.
Preset/localized copy from [references/presets.json](../data/onboarding/skills/sambl-onboarding/references/presets.json) is included;
do not refetch. Use the user's language (English fallback).

Use the supplied reference/version context as expectedVersion for child sambl/* loads,
including direct redirects. On reference_version_unavailable,
reload this entry without a pin; preserve choices and completed work, never replay Apply.

## Route the request

General capability questions call get_capabilities without identity, answer from
returned facts and stop: no file read, setup menu or task launch. Specific Theme,
Platform, Breakpoint, Collections, Palette and Slot tasks enter their available
sambl/themes, sambl/platforms, sambl/size-class, sambl/collections, sambl/palette
or sambl/slot-defaults entry through get_reference directly. Examples uses its
own entry. Collection-specific requests go straight to their native child,
without a parent recognition/setup phase. Do not add this introduction or
reinterpret child contracts.

For general setup, get_capabilities without identity once and use its actual
entryTool/reference actions. An empty list supplies no cause. Requested kit
preparation follows the selected child contracts; otherwise offer
copy.intro/copy.welcome once.
Basics needs a collection-setting or Slot action, Appearance needs Palette, and
Examples needs generate_examples. Capability questions reuse the returned list.
Documentation/history remain read-only without a kit. A selected task continues
directly, without another Configure step.

## Use the actual file and each child's access contract

Collections uses actual local collections, modes and relevant consumers. It has
no parent recognize_kit or version gate. Root metadata alone does not establish
or prohibit a structurally clear collection task. Resolve Core when migration or
another actual dependency needs it, not as a prerequisite for a subset or no-op.

For a selected child that uses STRICT SAMBL, follow the included shared admission
policy and that child's requirements. Reuse applicable same-task root facts and
recognized identity without repeating reads. Palette, Slots and Examples retain
their own admission contracts; native Collections does not acquire their gates.
Refine capabilities with a recognized identity only when the selected child needs it.

Read the actual local collection/mode catalogue as needed for the preparation
choices. A failed read is an error, not an empty catalogue. Missing collections
remain absent; Core-only means there are no remaining mode collections to
configure, not proof of which modes were selected earlier or a foreign-file claim.
Keep the target file and resolved choices with the task. On a file change, use
the new file's facts and the relevant child's access contract rather than reuse
stale choices or another file's result.

## Plan only existing collections

Build one preparation plan from the user's goal and actual catalogue, excluding
the resolved service Core. Reuse supplied selections and gather the remaining
material choices together. The conversation has no mandatory Theme → Platform →
Breakpoints order; choose execution order from actual dependencies and refresh
affected facts after each collapse.
Match standard roles by a unique case-insensitive collection name, retaining its
actual spelling. Duplicate matches need resolution or a skipped item, not an
automatic rename or selection. A missing role stays absent; choices do not spill
into another role. Extra collections require other_collections. An unavailable
child blocks its dependent item, not all otherwise available preparation.

Preserve the original user's explicit selections separately per collection,
including additional collections. Never silently omit an explicitly requested
collection. For a missing requested collection or mode, explain what is absent
and ask only the unresolved choice or offer to leave it unchanged. Conflicting
aliases, conflicting selections or a new preset disagreeing with supplied choices
need one focused clarification; never silently overwrite the user's choice.

For each unresolved collection choice, use its localized question from the delivered
data and offer only named presets whose entire exact mode set exists. For generic
collections substitute only the actual name into {collection}. Do not intersect a preset silently, translate mode names or restore
removed modes. Always allow Keep current settings and Custom; Single chooses one
actual mode. One selected mode collapses the non-Core collection, even if
it was the only existing mode or selected through Select all; explain that
consequence within the requested task. Keep current settings leaves it alone,
not a normalization or configured claim. With custom/renamed Theme modes, support keeping several modes too.
Custom uses the host user-choice rule with multiple selection of actual mode names; derive the count
from the selection, never ask it separately. Treat names such as Cancel or
constructor as literal mode names, not commands. Keep conversation actions
separate from data values. A “single Theme” choice belongs only to Theme.

After collection choices, use the matching sambl/themes, sambl/platforms,
sambl/size-class or sambl/collections entry at this entry's expectedVersion.
Keep the same file, actual names and resolved selections. Their included common
Collections knowledge describes native outcomes, not a server workflow or a new
Apply sequence. One retained mode migrates all variables except `name` to Core
and removes the matching component axis while preserving surviving instances.
Several retained modes keep the collection and corresponding component options.

An understandable preparation plan can already express the user's bounded
choices. Ask a replacement only when actual retired-mode/variant uses have
several unresolved destinations; no such uses means no fallback question. Refresh
facts affected by earlier changes, preserving the remaining intent. A real
collision, missing component branch or unpreservable override needs a focused
choice, not an initial migration questionnaire.

## Optional Slots and child execution

Include optional Slots in this preparation plan, including Core-only. If explicitly skipped or slot_defaults is
unavailable, continue to collections. Otherwise retrieve sambl/slot-defaults through
get_reference with the same expectedVersion and follow its complete skill with
actual same-task/file admission. Before offering copy.slots, use its read-only
onboarding readiness check; reuse only an applicable same-task/file verified result.
For already-configured (or reused configured), say the verified eligible Slots
are prepared, retain every omission/warning and continue without ensure/repair.
Nonblocking protected-list warnings do not become a new repair task. Never imply omitted definitions were prepared or all
original components remain. No eligible scope is unavailable, not ready; continue
the checklist with an honest notice. A sole PREPARATION_REQUIRED conflict permits
the ordinary copy.slots question even with protected-list warnings. Preserve an
explicit Prepare/Skip choice. Preserving manual settings is compatible with
Prepare: keep protected lists and prepare the eligible empty Slots with the child.
An explicit Skip still skips preparation. Prepare authorizes only canonical source
preferences/restrictions without a second Apply, preserving layouts/content.
Inspect or loading instructions grants no writes. Other conflicts
follow the child's focused handling, never ordinary Prepare. An incomplete,
blocked, failed or cancelled optional step may continue with an honest notice;
never mark it configured, retry automatically or hide partial changes. A prior
chat or cached flag is not readiness evidence. Missing helper never permits
installation/reconstruction.

Retain the Slot skill's actual native result locally; it has no workflow/report
callback. Native Collections likewise returns its actual same-file result to
this plan. Later child work uses the surviving components and real properties;
do not assume a pinned Slot index still resolves a changed backing or set.
For Palette retain its file, choices, handle and original responses and follow
its actual continuations and cleanup. A mismatched late result does not advance
the plan; local progress is not a parent workflowOutcome or server completion.

Retrieve pinned sambl/palette for its own intake, server calculation, choices and
Apply/Cancel/reportSpec/reportReady contract; do not reproduce it here. Examples
uses get_example_package and its entry, not a collection-style report callback.

Continue from the exact child's actual same-file outcome. Where the child uses
an operation, its actual continuation/terminal response still applies. For native
Collections summarize retained modes, actual changes and meaningful unresolved
issues without a separate report callback or mandatory postflight. Absence means
reassess the current catalogue, not infer a completed collapse.

Partial, failed or unknown work stops its dependent items; state what finished,
what may have changed and what remains unresolved. Preserve earlier results and
other independent requests. An active old operation still needs safe
reconciliation, not abandonment or replay. A return uses fresh relevant facts.
If the user stops a step before changes, retain earlier completed work and say
copy.cancelledStep. After work began, describe the actual partial or uncertain
outcome rather than claim a clean cancellation or whole-kit rollback.
Continue independent requested items whose scope remains valid, asking only
when the remaining goal is unresolved.

## Finish from actual outcomes

Track changed, already satisfied, kept/skipped, absent and unresolved from actual
child results, never local progress as server verification. Summarize visited
collections and returned retained modes; ending the checklist does not prove an
axis is configured. All-skipped keeps current settings; Core-only has no mode collections.
Failed/partial stays unfinished. Retain warnings and incomplete optional Slots.

If Palette was already requested, start that available dialogue with supplied
choices immediately after collection setup; do not add a Customize palette button
or ask again whether to start. Otherwise, after successful/kept collection setup,
offer only the optional copy.customizePalette action when available. No mandatory
Finish/Done/Continue or repeated introduction. No reply ends the conversation.
Do not start Examples automatically. A selected Examples request hands off to its
entry skill under its own access/adaptation contract, retaining the actual
screen request.

## Host user choices (included)

Keep actual names and choices; literal Cancel is data. Use the supplied service
values. Ask material unresolved choices through the host adapter.
A supplied resolved-input Start continues the task, not replay.

## Shared admission policy (included)

# Shared current-file admission policy

Included; do not refetch sambl/kit-admission. Applies only to admission-requiring
entries; onboarding follows its child. Native Collections uses its own knowledge.
General help/capabilities/changelog need no file.

Choose the route before file reads. Use the actual Design file; ask to open/select
one only when unavailable, never for technical IDs.

For palette_operation or variable_operation, Start owns STRICT
SAMBL admission: host root read plus recognize_kit for the action. Send known typed
choices, omit unresolved fields and follow input_required/inspection. No client
metadata read/recognize_kit prerequisite, even after onboarding. Continue exact
workflow/next, not another recognition/Start. Blocked/error stops; no fallback/repair.
Support is not readiness, native availability or Apply permission.

For version/compatibility questions and direct entries that require admission,
including Slots, Examples and existing semantic value edits,
read exact root sambl/kit-metadata natively. Call recognize_kit with protocolId
sambl-connector, contractVersion 0.1.0, unchanged metadataValue (including real empty)
and declared requestedCapability. Only this classifier interprets support, on host
or client; no local parsing/version lists/naming inference, repair or installation.
Actual read/tool errors stop with observed reasons; unattempted is not unavailable/empty.

Direct admission needs status ok/result.status recognized and the action's
checkedCapability. Blocked observedIdentity explains a version, never admits work.
Reuse fresh same-task/file evidence for its checked action. Another direct action
reuses retained raw metadata in recognize_kit; operation children use Start.
File/metadata change or uncertainty invalidates related results/choices. Recognition
proves neither unchanged design nor bindings; host/native freshness guards remain.

Setup children requiring admission and variable creation use STRICT SAMBL:
missing/foreign/malformed/unsupported metadata or actions stop before adaptation
or foundation creation.
Explain the actual reason/unsupported declared version plainly, not raw metadata/IDs.
Show maintained kitLink.kitRequired and Community data when relevant.
Examples alone owns informed Adapt/Cancel, including recognized versions without
a compatible Examples profile. This does not grant adaptation to setup skills.
No admission, instruction retrieval or mode choice is Apply permission.

Use only kitLink.communityKitUrl and communityLabel. When null, show
communityPending as plain text; never guess a URL. Preserve each operation's
actual approval/report contract.

## Resolve the service Core collection

For Palette, read local collection headers and exact SharedPluginData
sambl / collection-role strings. Its versioned Core marker is
{"schemaVersion":1,"role":"core"}. A unique valid marker on a local non-extension
collection identifies the service Core collection even if its display name was
changed. Protect its actual ID from configuration and preserve its display name.
Another collection named Core is not protected when the marker identifies a
different collection.

Read every role value successfully; an omitted or failed read is not an empty marker.
If every collection returns an empty role marker, support existing prepared
copies by resolving exactly one case-insensitive core name. Do not stamp a marker,
rename collections or infer Core from contained variables. Malformed/unsupported
nonempty markers, several marked Core collections, a marked extension/remote
collection or an ambiguous/missing legacy Core stop with the actual reason.
This role identifies the service destination; it grants no repair permission
and does not replace required Sambl kit recognition. Marker and unique-name
fallback are alternatives, not collections to merge.

# Feedback
If enabled, offer sambl/feedback once for unsupported/poor Sambl results. No auto-send or contact intake.

## Delivered preset data

```json
{"format":"sambl-onboarding-presets-v1","copy":{"intro":{"en":"Sambl is a versatile UI kit for Figma, with agent workflows that take care of routine setup.","ru":"Sambl — универсальный UI-кит для Figma с агентскими сценариями, которые берут на себя рутинную настройку."},"welcome":{"question":{"en":"Where would you like to start?","ru":"С чего начнём?"},"choices":[{"key":"basics","label":{"en":"Set up the basics (themes, breakpoints, platforms)","ru":"Настроить общие характеристики (темы, брейкпоинты, платформы)"}},{"key":"appearance","label":{"en":"Customize appearance (change the palette)","ru":"Настроить внешний вид (изменить палитру)"}},{"key":"examples","label":{"en":"Add an example screen","ru":"Добавить пример экрана"}},{"key":"capabilities","label":{"en":"See what Sambl can do","ru":"Посмотреть возможности Sambl"}}]},"slots":{"question":{"en":"Prepare the slots?","ru":"Подготовить слоты?"},"prepare":{"en":"Prepare slots (recommended)","ru":"Подготовить слоты (рекомендуется)"},"skip":{"en":"Skip for now","ru":"Пока пропустить"},"intro":{"en":"I’ll set up preferred content for slots to make components easier to configure. Your layouts won’t change.","ru":"Настрою подсказки для слотов. Это упростит настройку компонентов и не изменит макеты."}},"cancelledStep":{"en":"Changes from this step were not applied. Earlier completed changes remain.","ru":"Изменения этого шага не применены. Ранее выполненные изменения сохранены."},"customizePalette":{"en":"Customize palette","ru":"Настроить палитру"}},"roles":[{"collection":"theme","capability":"themes","question":{"en":"Which themes does your product need?","ru":"Какие темы нужны вашему продукту?"},"presets":[{"key":"system","label":{"en":"Light & dark (default)","ru":"Светлая и тёмная (по умолчанию)"},"modes":["light","dark"]},{"key":"single","label":{"en":"Single theme","ru":"Одна тема"},"selection":"single"},{"key":"custom","label":{"en":"Custom","ru":"Свой вариант"},"selection":"multiple"},{"key":"keep","label":{"en":"Keep current settings","ru":"Оставить текущие настройки"},"selection":"keep"}]},{"collection":"platform","capability":"platforms","question":{"en":"Which platforms does your product need?","ru":"Какие платформы нужны вашему продукту?"},"presets":[{"key":"cross-platform","label":{"en":"Cross-platform (default) · Web + mobile","ru":"Кроссплатформенный (по умолчанию) · Web + мобильные"},"modes":["apple","android","web"]},{"key":"mobile","label":{"en":"Mobile · iOS & Android","ru":"Мобильный · iOS и Android"},"modes":["apple","android"]},{"key":"single","label":{"en":"Single platform","ru":"Одна платформа"},"selection":"single"},{"key":"custom","label":{"en":"Custom","ru":"Свой вариант"},"selection":"multiple"},{"key":"keep","label":{"en":"Keep current settings","ru":"Оставить текущие настройки"},"selection":"keep"}]},{"collection":"size-class","capability":"size_classes","question":{"en":"Which breakpoints does your product need?","ru":"Какие брейкпоинты нужны вашему продукту?"},"presets":[{"key":"all-breakpoints","label":{"en":"Responsive (default)","ru":"Адаптив (по умолчанию)"},"modes":["sm","md","lg","xl"]},{"key":"desktop-mobile","label":{"en":"Desktop + Mobile","ru":"Десктоп + мобильные"},"modes":["sm","xl"]},{"key":"mobile-only","label":{"en":"Mobile only","ru":"Только мобильные"},"modes":["sm"]},{"key":"desktop-only","label":{"en":"Desktop only","ru":"Только десктоп"},"modes":["xl"]},{"key":"custom","label":{"en":"Custom","ru":"Свой вариант"},"selection":"multiple"},{"key":"keep","label":{"en":"Keep current settings","ru":"Оставить текущие настройки"},"selection":"keep"}]}],"otherCollections":{"capability":"other_collections","question":{"en":"Which {collection} setup fits your product?","ru":"Как настроить {collection} для вашего продукта?"},"presets":[{"key":"single","label":{"en":"Single mode","ru":"Один режим"},"selection":"single"},{"key":"custom","label":{"en":"Custom","ru":"Свой вариант"},"selection":"multiple"},{"key":"keep","label":{"en":"Keep current settings","ru":"Оставить текущие настройки"},"selection":"keep"}]},"kitLink":{"communityKitUrl":"https://www.figma.com/community/file/1694910886681282187/sambl-ui-kit","kitRequired":{"en":"Sambl setup works only with a supported copy of Sambl UI Kit. Open a copy of the Community kit to continue.","ru":"Настройка Sambl работает только с поддерживаемой копией Sambl UI Kit. Чтобы продолжить, откройте копию кита из Community."},"communityLabel":{"en":"Sambl UI Kit on Figma Community","ru":"Sambl UI Kit в Figma Community"},"communityPending":{"en":"Sambl UI Kit on Figma Community — link coming soon","ru":"Sambl UI Kit в Figma Community — ссылка появится позже"}}}
```
