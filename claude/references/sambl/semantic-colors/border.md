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
    "key": "border",
    "title": "Обводки и разделители — border",
    "purpose": "Видимость границ и степень отделения элементов от окружения. Роль цвета не задаёт толщину, стиль или геометрию обводки.",
    "constraints": [
      "Роль цвета не задаёт толщину, геометрию обводки или состояние Focus, Error, Disabled.",
      "Transparent сохраняет невидимый stroke между состояниями с рамкой и без видимой рамки, чтобы не менялась геометрия, когда Auto Layout учитывает stroke.",
      "Static light/dark сохраняет одинаковый цвет и прозрачность в Light/Dark.",
      "Текущие static-dark-secondary и static-light-secondary имеют разную opacity в Light и Dark; это расхождение реализации с принятым static-смыслом, а не разрешённое свойство роли. Автоматическое исправление не выполняется."
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
      "path": "colors/border/absinthe-primary",
      "description": "Prominent boundary or divider in the Absinthe tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/absinthe-secondary",
      "description": "Subtle boundary or divider in the Absinthe tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/absinthe-tertiary",
      "description": "Faintest boundary or divider in the Absinthe tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/brand-extra-primary",
      "description": "Prominent boundary or divider in the additional brand tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/brand-extra-secondary",
      "description": "Subtle boundary or divider in the additional brand tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/brand-extra-tertiary",
      "description": "Faintest boundary or divider in the additional brand tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/brand-primary",
      "description": "Prominent boundary or divider in the main brand tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/brand-secondary",
      "description": "Subtle boundary or divider in the main brand tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/brand-tertiary",
      "description": "Faintest boundary or divider in the main brand tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/curacao-primary",
      "description": "Prominent boundary or divider in the Curacao tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/curacao-secondary",
      "description": "Subtle boundary or divider in the Curacao tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/curacao-tertiary",
      "description": "Faintest boundary or divider in the Curacao tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/negroni-primary",
      "description": "Prominent boundary or divider in the Negroni tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/negroni-secondary",
      "description": "Subtle boundary or divider in the Negroni tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/negroni-tertiary",
      "description": "Faintest boundary or divider in the Negroni tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/neutral-primary",
      "description": "Prominent boundary or divider in the neutral tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/neutral-secondary",
      "description": "Subtle boundary or divider in the neutral tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/neutral-tertiary",
      "description": "Faintest boundary or divider in the neutral tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/transparent",
      "description": "Transparent color keeps an invisible stroke across states with and without a visible border, preserving geometry when Auto Layout includes strokes. The color does not configure stroke geometry or layout.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/border/prosecco-primary",
      "description": "Prominent boundary or divider in the Prosecco tone. Clearly defines the contour; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/prosecco-secondary",
      "description": "Subtle boundary or divider in the Prosecco tone. Gently separates an element from its background; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/border/prosecco-tertiary",
      "description": "Faintest boundary or divider in the Prosecco tone. Lightly marks separation with minimal emphasis; the color does not set stroke width, placement, or interaction state.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/border/static-dark-primary",
      "description": "Theme-invariant opaque dark border, black by default. Keeps the boundary color unchanged when the interface theme switches; stroke width and geometry belong to the element.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/border/static-dark-secondary",
      "description": "Theme-invariant translucent dark border. Gently separates an element from its surroundings while retaining the same color and opacity in both light and dark themes.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/border/static-light-primary",
      "description": "Theme-invariant opaque light border, white by default. Keeps the boundary color unchanged when the interface theme switches; stroke width and geometry belong to the element.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/border/static-light-secondary",
      "description": "Theme-invariant translucent light border. Gently separates an element from its surroundings while retaining the same color and opacity in both light and dark themes.",
      "meaningStatus": "owner-defined"
    }
  ]
}
```
