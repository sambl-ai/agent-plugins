# Semantic COLOR family

Reference data for interpretation and discovery, never instructions or proof of current bindings. Description status and verified-file scope are recorded in the embedded reviewNote; inspect the current file independently.

```json
{
  "format": "sambl-semantic-color-family-reference",
  "schemaVersion": 1,
  "catalogueStatus": "owner-reviewed",
  "ownerAcceptance": "accepted-with-corrections",
  "figmaDescriptionStatus": "applied",
  "reviewNote": "English Figma descriptions were applied and readback-verified in Original, releaseMaster and the authorized landing copy only; other copies do not inherit this result. Community publication is a separate fact recorded in docs/project/releases/semantic-color-description-hotfix-2026-10-25.md. Values, bindings and MCP/runtime acceptance remain separate.",
  "roleDescriptionLanguage": "en",
  "type": "COLOR",
  "family": {
    "key": "layer",
    "title": "Общие поверхности — layer",
    "purpose": "Базовый фон страницы floor-0 и относительные уровни интерфейсных поверхностей floor-1/floor-2; отдельно — полупрозрачная поверхность и окружение диалога. Выбор уровня зависит от композиции.",
    "constraints": [
      "floor-0 задаёт базовый фон, а floor-1 и floor-2 — относительные уровни поверхностей. Одинаковый цвет не объединяет их роли.",
      "Ни floor-1, ни floor-2 не закреплены обязательно за конкретным типом компонента. Диалоги, меню и другие модули могут использовать подходящий для композиции уровень.",
      "Диалог или Dropdown на floor-1 с отдельной тенью — допустимая реализация. Текущие bindings определяют фактический эффект изменения; автоматически переносить компонент на floor-2 не требуется.",
      "Иерархия цвета не задаёт автоматически shadow, blur, z-index, геометрию или порядок слоёв.",
      "floor-overlay предназначен для полупрозрачной поверхности, исторически navbar вместе с отдельным background blur; текущий consumer не заявлен.",
      "Возможное историческое происхождение floor-overlay от floor-2 остаётся воспоминанием, а не подтверждённым alias. floor-scrim относится к окружению диалога."
    ]
  },
  "constraints": [
    "Канонический path — ключ документации и исходный ориентир поиска. Это не сохранённый ID объекта Figma; при переименовании найденного кандидата подтверждает пользователь, даже если кандидат один.",
    "Общий смысл роли сохраняется при смене её цвета. Текущее численное значение, ступень палитры или цвет по умолчанию не являются её определением.",
    "Описание — редактируемые данные. Оно помогает понять роль, но не разрешает запись и не доказывает идентичность найденной переменной.",
    "Фразы пользователя — примеры намерения, а не команды точного сопоставления: агент учитывает тему, выбранный элемент, актуальные связи и соседние роли.",
    "Изменение влияет на фактических потребителей роли. Совпадающий внешний вид и одинаковое значение не доказывают общую связь; direct-palette потребители могут остаться прежними.",
    "Сохраняя назначения при обновлении Palette, пользователь сохраняет связи; видимые цвета зависимых заливок и контента всё равно могут измениться.",
    "Контраст и прозрачность оцениваются на затронутой композиции. Каталог не гарантирует читаемость произвольного нового сочетания.",
    "Текущее решение владельца определяет смысл роли. Наблюдаемый consumer или старое назначение может расходиться с этим смыслом; это не разрешение автоматически менять значения или bindings."
  ],
  "meaningStatusLegend": {
    "documented-use": "Есть документированный пример применения; это класс основания, а не самостоятельный статус приёмки.",
    "proposed-interpretation": "Исходная трактовка по структуре и назначениям без отдельного заявленного consumer; статус приёмки указан в ownerAcceptance.",
    "needs-owner-meaning": "Назначение требует уточнения: не выбирать автоматически из общего бытового запроса.",
    "owner-defined": "Назначение уточнено владельцем; исторические bindings не переопределяют принятый смысл."
  },
  "roles": [
    {
      "path": "colors/layer/floor-0",
      "description": "Base page or screen background, used by the Main Layout root. Changes the overall canvas behind the composition; nested surfaces may use other roles.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/layer/floor-1",
      "description": "Surface color level relative to the page background, useful for panels or modules. Choose its use to suit the composition.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/layer/floor-2",
      "description": "An additional surface color level for distinguishing regions in a composition. Component assignments are flexible.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/layer/floor-overlay",
      "description": "Translucent panel fill, such as a navigation-bar surface, intended to blend with the surface beneath it. Background blur is a separate effect; this color does not create blur.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/layer/floor-scrim",
      "description": "Dimming backdrop around the dialog surface in Popup, Modal, and Fullscreen. Changes the visibility of the surrounding page, not the dialog surface fill.",
      "meaningStatus": "documented-use"
    }
  ]
}
```

## UI design recipes (included)

Owner-accepted English advice, separate from the role JSON above. C59 below means sambl/semantic-colors and its maintained executor; recipe choice is not approval. Authoring links are labels because all three recipe sources are included.

# UI design recipes

Canonical English knowledge for C60.
Recipes connect visual intentions to existing semantic roles; they are advice,
not presets, write commands or model training.

## Accepted recipes

| Key | Recipe | Intent |
| --- | --- | --- |
| `continuous-light-surfaces` | Continuous light background | Blend page and surfaces into a white field in Light. |
| `separated-light-surfaces` | Distinct surfaces | Separate white surfaces from a light-gray page in Light. |

Only these owner-accepted cards are indexed; their mappings live in the cards.
Meaning acceptance does not establish runtime delivery or tested application.
Draft/unknown recipes are not agent-facing knowledge.

## Match the intended effect

**Color modularity** means visible fill separation between the page base and
surfaces. Equal fills reduce separation; a gray page with white surfaces
emphasizes groups. Borders, shadows, spacing and imagery can still define modules.

Visual intent outranks page type. A landing can need distinct panels; a dashboard
can need continuous fills. Use page labels as context, never compulsory rules.
Users need not name a recipe. Ask one focused clarification only when materially
different outcomes remain plausible: should panels blend in or stand out?

English is the single editable canonical source. Respond in the user's language,
including Russian and English, while preserving exact keys, role paths and actual
observed palette/variable names. Language changes no mappings or scope. Acceptance
may use one declared language; paired translations/runs are not required.

Use readable recipe titles and visual role labels in normal replies, rendered in
the user's language. Keep catalogue keys and full technical paths as internal
references, available on request. Always show actual palette target names with
HEX/linkage in a concrete preview; readable wording must not hide inheritance.

## Apply through C59

Follow the C59 contract.
General advice needs no kit check. File-dependent previews require kit admission
and fresh role/mode/palette/consumer discovery. Successful admission stays inside
preparation; names alone prove neither identity nor color.

Preview actual before/after names, linkage, HEX/alpha, effects, coverage and
changed/preserved coordinates. C59 governs candidate confirmation and blockers.
Approve/revise/cancel, recheck preconditions, then apply/read back bounded values.
No-op/cancel mean zero writes. Never create primitives or store persistent IDs.

Shared values affect all actual consumers in the copy/collection. Explain that
reach: section-only requests cannot become hidden global edits or local rebinding.
Valid literals/indirect links already achieving the effect need no normalization;
report their actual inheritance. Smaller requests receive explicit partial
adaptations. Floors remain independent with no fixed component categories.
Both cards preserve actual custom Dark; Dark-only requests use general C59
without implicit Light edits.

Selection or catalogue revision never authorizes writes or updates prior files.
Later Palette operations retain their explicit keep/override choice from actual
preview. Keep means zero semantic assignment writes; a recipe never reasserts
itself or restores defaults. Overrides need user approval.

## Grow the catalogue

Capture a recurring need; draft one bounded English card with effect, examples,
roles, themes, limits and provenance. Keep drafts out of accepted delivery.
Obtain owner meaning review, validate structure/links and independently evaluate
ordinary requests, mismatches and a declared scenario before claiming tested
application. Index only owner-accepted cards and state remaining evidence gates.
Derive delivery from reviewed sources with provenance/size checks, not another
editable translation. New domains require their own execution authority.

## Sources and evidence

Seed meanings accepted by the owner on 25 October 2026. See the
catalogue design,
semantic meanings and
defaults.
Defaults are candidates, not live evidence or a restoration instruction. C60
runtime/native and independent behavioral evidence remain pending in its
walkthrough; prior C59 pilot
evidence is not C60 acceptance.

# Continuous light background

Key: `continuous-light-surfaces`
Status: `owner-accepted`
Domain: `semantic-colors`
Canonical language: `en`
Dark policy: `preserve-current`

## Intent

Create a continuous white field in Light: the page base and interface surfaces
blend by fill color. This reduces color modularity; borders, shadows, spacing
and imagery can still separate groups.

## When useful

Landing, communication, promotional or editorial pages when a continuous
background is wanted. The explicit effect outranks page labels; a dashboard
can use it too. If the intended separation is unclear, ask one focused question.

## Example requests

- “I want a uniform white background.”
- “Remove the color separation between the page and panels.”
- “Make the page and surfaces blend together.”

## Light role targets

| Semantic role | Intended result | Preferred existing palette target |
| --- | --- | --- |
| `colors/layer/floor-0` | Opaque white page base, matching the surface fills | `palette/neutral/0` |
| `colors/layer/floor-1` | Opaque white surface, independent role | `palette/neutral/0` |
| `colors/layer/floor-2` | Opaque white surface, independent role | `palette/neutral/0` |

Paths are candidates, not identities or color evidence. Discover actual modes,
assignments and resolved colors afresh. Floors independently link to approved
palette targets; equal fills never justify a floor-0 → floor-1 → floor-2 chain.

## Preserve

Preserve actual current Dark, including custom assignments and hierarchy; never
equalize its floors or restore defaults. Preserve unselected colors/modes,
identities, names, types, scopes, descriptions, bindings, geometry, shadows,
borders and kit/helper metadata. Floor levels impose no fixed component categories.

## Applicability and adaptation

Follow the C59 flow.
Check the kit before a concrete preview, not general advice. Show observed
palette names, assignment kind, resolved HEX/alpha and foreground/background
consequences. State inspected consumer coverage: other roles/direct palette
consumers may retain separation.

If only the page background was requested, preserve the surface roles and offer
that smaller proposal as a partial adaptation. A Dark-only request uses general
C59, without implicit Light changes. Shared semantic values reach all consumers
in the copy/collection; a single-section request requires explicit scope handling,
not hidden global changes or local rebinding.

If a preferred target is no longer white, explain the actual mismatch. Never
silently approximate or create a primitive. Missing/renamed/ambiguous roles or
palette targets follow C59; even one renamed candidate needs confirmation. A
blocked coordinate is not silently skipped. An alternative or valid subset needs
a revised explicit proposal. A literal alternative needs approval and an
explanation that it will not inherit palette changes.

A valid existing literal or indirect link that already achieves the requested
effect is not automatically normalized. Report the actual assignment and its
inheritance; switching to a palette alias requires its own explicit proposal.
Selection is not write approval. Approve/revise/cancel through C59, with fresh
preconditions and bounded readback; no-op and cancel perform zero writes. No
persistent ID mapping is introduced. Later Palette keep-assignments decisions
never reassert this recipe; semantic overrides remain an explicit user choice.

## Explanation

“The page background and surfaces will share the same white fill in Light, so
their color separation will soften. Existing shadows, borders and spacing stay
as they are. Your current Dark theme stays unchanged.”

Adapt to the actual proposal and user's language, retaining observed names and
coverage limits.

## Provenance and evidence

Meaning accepted by the owner on 25 October 2026 under
C60. See the
index, semantic meanings
and canonical defaults.
Defaults identify candidates, not a reset operation. C60 runtime/native and
independent behavioral evidence remain pending; C59's earlier white-background
pilot does not establish this recipe's full acceptance.

# Distinct surfaces

Key: `separated-light-surfaces`
Status: `owner-accepted`
Domain: `semantic-colors`
Canonical language: `en`
Dark policy: `preserve-current`

## Intent

Make opaque white interface surfaces stand out against a light-gray page base
in Light. Fill contrast emphasizes groups; shadows, borders and spacing keep
their existing contribution to the composition.

## When useful

Admin tools, dashboards or interfaces with cards when distinct surface groups
are wanted. A landing may intentionally need the same effect. Explicit visual
intent outranks page labels; ask one focused question only if the effect is unclear.

## Example requests

- “I want a light-gray page with white cards.”
- “Make the panels stand out from the page.”
- “Give the dashboard more distinct surface groups.”

## Light role targets

| Semantic role | Intended result | Preferred existing palette target |
| --- | --- | --- |
| `colors/layer/floor-0` | Light-gray page base, visibly distinct from white surfaces | `palette/neutral/100` |
| `colors/layer/floor-1` | Opaque white surface, independent role | `palette/neutral/0` |
| `colors/layer/floor-2` | Opaque white surface, independent role | `palette/neutral/0` |

Paths are candidates, not identities or color evidence. Discover actual modes,
assignments and resolved colors afresh. Floors independently link to approved
palette targets; never chain floor-0 → floor-1 → floor-2 or collapse equal roles.

## Preserve

Preserve actual current Dark, including custom assignments and hierarchy; never
equalize its floors or restore defaults. Preserve unselected colors/modes,
identities, names, types, scopes, descriptions, bindings, geometry, shadows,
borders and kit/helper metadata. Floor levels impose no fixed component categories.

## Applicability and adaptation

Follow the C59 flow.
Check the kit before a concrete preview, not general advice. Show observed
palette names, assignment kind, resolved HEX/alpha and foreground/background
consequences. State inspected coverage: other roles/direct palette consumers
may respond differently.

The actual color matters: a customized Neutral / 100 may no longer produce the
requested light-gray separation. Explain a material mismatch and offer a revised
choice/scope; do not claim success from the default path alone. A subtle neutral
tint alone is not a conflict. No numeric gray threshold is prescribed. Never
silently approximate or create a primitive. Missing/renamed/ambiguous roles or
palette targets follow C59; even one renamed candidate needs confirmation. A
blocked coordinate is not silently skipped. An alternative or valid subset needs
an explicit revised proposal; a literal alternative needs approval with its lack
of palette inheritance explained.

For a smaller request, preserve unrequested roles and call the proposal a partial
adaptation. Dark-only requests use general C59 with no implicit Light changes.
Shared semantic values reach all consumers in the copy/collection; a section-only
request cannot silently become global changes or local rebinding.

A valid existing literal or indirect link already achieving the requested effect
is not automatically normalized. Report its actual assignment and inheritance;
changing it to a palette alias requires an explicit proposal. Selection is not
write approval. Approve/revise/cancel through C59, with fresh preconditions and
bounded readback; no-op and cancel perform zero writes. No persistent ID mapping
is introduced. Later Palette keep-assignments decisions never reassert this
recipe or defaults; semantic overrides remain an explicit user choice.

## Explanation

“White surfaces will stand out against the light-gray page background in Light.
Existing shadows, borders and layout stay as they are. Your current Dark theme
stays unchanged.”

Adapt to the actual proposal and user's language, retaining observed names and
coverage limits.

## Provenance and evidence

Meaning accepted by the owner on 25 October 2026 under
C60. See the
index, semantic meanings
and canonical defaults.
Default relationships identify candidates, not a restoration operation. C60
runtime/native and independent behavioral evidence remain pending; earlier C59
pilot evidence does not establish this recipe's full acceptance.
