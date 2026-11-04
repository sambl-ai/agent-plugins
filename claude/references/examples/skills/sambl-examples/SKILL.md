---
name: sambl-examples
description: Guide Sign In or Dashboard requests through kit and foundation checks, optional informed adaptation and package retrieval, then build and self-check the result.
---

# Generate an example

This entry skill controls the conversation and continuation. get_example_package
only retrieves instructions and specifications; an entry_skill result is the
complete entry, not a missing screen or server failure. Retain this text before
asking the user anything. Do not load build references or make file changes yet.
The user names a screen, not its component inventory or expected layout.

## Recover entry delivery context

Continue directly when this complete entry arrived in a real entry_skill result
with its catalogue and packageVersion. Reading it through get_reference or a
Resource does not provide that wrapper. If either field is missing, first call
get_example_package with protocolId sambl-connector and
contractVersion 0.1.0, without screen or packageVersion. Retain its complete
entry_skill result, then continue that returned entry. Do not infer packageVersion
from the MCP protocol, this document's version label or a remembered release.
Preserve actual user choices, fresh file observations and completed owned work;
do not repeat an already answered question or replay construction. A complete
wrapped entry needs no extra retrieval merely to confirm that it is complete.

## Select and admit the actual file

Use the returned catalogue. Resolve Sign In or Dashboard from the user's request;
ask these two choices only when selection is missing or ambiguous. Keep Dashboard
as the public name and describe it as an example screen from a product dashboard.

Reuse an actual fresh same-task/file recognize_kit result only if it checked
requestedCapability generate_examples. Otherwise reuse the applicable exact raw
root observation, or read the actual current Design file root
getSharedPluginData("sambl", "kit-metadata") through native Plugin API JavaScript.
Call recognize_kit with protocolId sambl-connector, contractVersion
0.1.0, that unchanged metadataValue (including a real empty string), and
requestedCapability generate_examples. Only this tool parses metadata and checks
release/action/profile support. Never parse it locally or use a package catalogue
as an independent admission rule. A failed read stops
with its actual error; do not guess identity or install metadata/helpers.
Recognition checks metadata support, not source readiness. Inspect actual needed
dependencies after admission; retain the exact raw observation for native drift
checks and later child capability checks.

## Verify a usable foundation before continuing

Before offering Adapt, retrieving construction dependencies or making any writes,
read the actual relevant variable and text-style catalogues. First establish a
usable local foundation: existing suitable COLOR variables for element colors
and applicable existing text styles with usable fonts. Do not require exact
canonical token/style paths or the full dependency closure at this initial gate;
resolve the selected WHAT's detailed role mapping later, before any writes.
Arbitrary unrelated variables/styles do not satisfy this gate. A metadata pass,
matching names or a nonempty catalogue alone is not proof. Reuse fresh actual
same-file/task observations only while the relevant catalogues and requirements
remain unchanged; otherwise check again.

If either usable color variables or applicable text styles are absent, stop:
“I can’t generate this example here: it needs existing color variables and usable
text styles for its elements.” / “Не могу собрать пример в этом файле: для его
элементов нужны существующие цветовые переменные и подходящие текстовые стили.”
Name the missing foundation plainly and show Community information below. Do not
offer Adapt, load construction dependencies, create an Examples page/Sections,
prepare Slots or construct any elements. Never create variables/styles or use
literal paint/font formatting to compensate. A read/access/font-loading failure
is a distinct actual error, not proof that foundation data is absent. Preserve
its error and stop affected work instead of offering a bypass.

Only after this gate, for a recognized supported kit retain local build mode
sambl-kit and continue to package retrieval below. Do not ask for adaptation
merely because an individual preferred source was deleted; suitable existing
variables/styles and the documented substitution policy can still support it.

For missing, foreign, malformed or unsupported metadata, retain that distinction
and explain that canonical Examples cannot run. A returned observedIdentity only
reports a declared version, never admission. For capability_unsupported or
capability_profile_unavailable, explain that this kit version has no supported
Examples recipe/profile; do not call the whole file foreign or silently use
canonical mode. If and only if the foundation gate passed, offer a separate
adapted example using its available components, styles and variables, with no
promise of the Sambl reference result. Show Adapt / Cancel through the included
host user-choice rule and wait. Suggested wording:
“I can adapt Dashboard using this file’s variables and text styles, but the result
may differ from the Sambl example. Adapt the example to this file?” /
“Могу адаптировать Dashboard на переменных и текстовых стилях этого файла, но
результат может отличаться от примера Sambl. Адаптировать пример к этому файлу?”
Replace Dashboard with Sign In when selected.

For the foundation stop or this adaptation offer, use the delivered kitLink data:
when communityKitUrl is non-null, show that exact official URL with communityLabel
in the user's language; when null, show communityPending as plain text. Never
invent a Community URL or render the pending label as a link.

## Continue after the answer

Cancel stops without package loading or writes. The original generation request
is not adaptation consent. After explicit Adapt, retain local build mode adapted
and immediately call get_example_package on the same Sambl connector with
protocolId sambl-connector, contractVersion 0.1.0, screen set to the
selected catalogue key (dashboard or sign-in), and packageVersion from this entry.
No file key, metadata, consent token, action or report belongs in this call.
For recognized kits use that same package call directly after admission and the
foundation check. A selected screen always requires the returned packageVersion;
never omit it to request an unpinned current package.
Do not await another user prompt, repeat the consent question or treat the
absence of a package in the initial entry response as unavailability. If an
actual call fails, name that call and its actual error; do not invent a failure.

Recognition, foundation evidence, consent and mode stay local to this file and
request. A file or screen switch requires a new applicable check/choice; never
carry consent into another target. On a package/reference version mismatch, pause dependent work
and retrieve a fresh entry without screen or packageVersion; old packages are
not retained. Preserve real choices and completed work, then reconcile the current
requirements before continuing. Do not silently mix versions, repeat consent for
the same unchanged scope or automatically replay completed construction.

## Build and finish

Once the screen_package is returned, read its before-build packs in order, then
component WHAT only when needed. Packs contain complete documents; retain each
source under its original reference/path and do not fetch it again through links.
Resources and get_reference return identical bytes. For a Resource, require the
returned versioned URI to equal the screen_package URI. For a tool response,
require its version to equal that reference's version in the package. Retain this
version with the complete document. Use the supplied fallback request, including
expectedVersion, when Resources are unavailable or cannot establish the pinned
URI. Never omit the pin to bypass a mismatch. Follow the delivered assembly and
component skills.

After reading the selected WHAT, prove its required color and text roles can be
supplied by suitable existing local variables/styles, including any documented
substitutions. Do this before page/Section creation or dependent construction.
If required roles cannot be supplied, explain the exact gap
and stop affected work; neither Adapt nor a partial package permits creating
foundation variables/styles or using unbound color/font literals to bypass it.

Build/reuse the selected dependencies and screen using the actual sources and
consumer Slots they need. Full source Slot preparation is a separate task, not
an Examples prerequisite. Preserve source defaults and user-managed or unknown
preferred lists; unrelated recommendations do not block this output. Check the
selected dependencies' real Slot identities, settings, required content and native
consumer validity under the delivered Slot policy. A real required-content
violation remains a gap; a warning about another source is not a repair task.
In adapted mode use actual local components/styles/tokens and disclose
substitutions, without installing Sambl helpers or metadata. If required styling
has become unavailable, stop dependent writes; Adapt does not create foundations.
Preserve user content and actual native/provider restrictions.
Required behavior that cannot be supplied needs an honest gap or focused question.

Create/reuse the Examples page and only the selected screen with its dependencies.
Resolve relevant sources, styling, content and mode mappings once and reuse fresh
facts across specimens. Keep actual retained modes. Use the package baselineProfiles only as structural
composition mappings, never as the actual file mode inventory. Delivery version
pins do not determine whether existing output is compatible; check its current
relevant contract and actual owned state before reuse. Style the boards last.
Self-check and finish with real screen/component links, an invitation to view, actual problems and, for an
adaptation, its explicit adapted qualification. No final MCP report, Codex gate,
mandatory acceptance or automatic next screen is required. Honor narrower user
scope such as preparation without canvas writes. Retrieval itself grants no writes.

# Feedback
If enabled, offer sambl/feedback once for unsupported/poor Sambl results. No auto-send or contact intake.

## Host user choices (included)

Keep actual names and choices; literal Cancel is data. Use the supplied service
values. Ask material unresolved choices through the host adapter.
A supplied resolved-input Start continues the task, not replay.

## Connection interruption (included)

Preserve accepted results. Use supplied status in the same scope and its read
request for missing approved data. Inspect actual state; never replay Start/Apply.
Only known-stopped work under active original approval may finish proven missing
changes within existing guards. Otherwise use reads and known-stopped reporting
only. Completed work needs no writes. Status renews nothing. Stopped work permits
saved-report acknowledgement and owned cleanup; cleanup errors preserve accepted
results. If pending at turn end, offer “check completion” on continuation.

## Delivered Community link data

```json
{"kitLink":{"communityKitUrl":"https://www.figma.com/community/file/1694910886681282187/sambl-ui-kit","kitRequired":{"en":"Sambl setup works only with a supported copy of Sambl UI Kit. Open a copy of the Community kit to continue.","ru":"Настройка Sambl работает только с поддерживаемой копией Sambl UI Kit. Чтобы продолжить, откройте копию кита из Community."},"communityLabel":{"en":"Sambl UI Kit on Figma Community","ru":"Sambl UI Kit в Figma Community"},"communityPending":{"en":"Sambl UI Kit on Figma Community — link coming soon","ru":"Sambl UI Kit в Figma Community — ссылка появится позже"}}}
```
