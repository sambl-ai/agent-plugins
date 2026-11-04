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
    "key": "content",
    "title": "Текст и иконки — content",
    "purpose": "Визуальная иерархия содержимого, контент на выраженной или противоположной по светлоте поверхности и цвета, независимые от переключения темы.",
    "constraints": [
      "Primary, secondary и tertiary описывают иерархию содержимого; tertiary не означает автоматически Disabled.",
      "Semantic Content Tertiary отличается от Tone Surface Variant Tertiary: часть компонентных рецептов обращается прямо к палитре.",
      "On-tone относится к тексту и иконкам поверх выраженных заливок; их контраст проверяется вместе с фактическими заливками и состояниями.",
      "Static сохраняет одинаковый цвет и прозрачность в Light/Dark, часто для текста и иконок поверх изображений или другого содержимого, не зависящего от темы. Inverted обозначает обратную композицию, а не вычисление инверсии RGB."
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
      "path": "colors/content/absinthe-primary",
      "description": "Main text and icons in the Absinthe tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/absinthe-secondary",
      "description": "Supporting text and icons in the Absinthe tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/absinthe-tertiary",
      "description": "Text and icons with the least emphasis in the Absinthe tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-extra-primary",
      "description": "Main text and icons in the additional brand tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-extra-secondary",
      "description": "Supporting text and icons in the additional brand tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-extra-tertiary",
      "description": "Text and icons with the least emphasis in the additional brand tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-primary",
      "description": "Main text and icons in the main brand tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-secondary",
      "description": "Supporting text and icons in the main brand tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/brand-tertiary",
      "description": "Text and icons with the least emphasis in the main brand tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/curacao-primary",
      "description": "Main text and icons in the Curacao tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/curacao-secondary",
      "description": "Supporting text and icons in the Curacao tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/curacao-tertiary",
      "description": "Text and icons with the least emphasis in the Curacao tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/negroni-primary",
      "description": "Main text and icons in the Negroni tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/negroni-secondary",
      "description": "Supporting text and icons in the Negroni tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/negroni-tertiary",
      "description": "Text and icons with the least emphasis in the Negroni tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/neutral-primary",
      "description": "Main text and icons in the neutral tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/neutral-primary-inverted",
      "description": "Main neutral text and icons on a surface with the opposite lightness to the usual neutral composition. Supports an inverted composition; does not calculate an RGB inverse.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/content/neutral-secondary",
      "description": "Supporting text and icons in the neutral tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/neutral-tertiary",
      "description": "Text and icons with the least emphasis in the neutral tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-absinthe",
      "description": "Text and icons over strong Absinthe fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-brand",
      "description": "Text and icons over strong main brand fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-brand-extra",
      "description": "Text and icons over strong additional brand fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-curacao",
      "description": "Text and icons over strong Curacao fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-negroni",
      "description": "Text and icons over strong Negroni fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-neutral",
      "description": "Text and icons over strong neutral fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/on-prosecco",
      "description": "Text and icons over strong Prosecco fills. Supports readable content on those surfaces; changes need to be considered together with the actual fills.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/prosecco-primary",
      "description": "Main text and icons in the Prosecco tone. Establishes the primary level of emphasis; changes affect labels and graphics bound to this role.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/prosecco-secondary",
      "description": "Supporting text and icons in the Prosecco tone. Carries secondary information with less emphasis than primary content; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/prosecco-tertiary",
      "description": "Text and icons with the least emphasis in the Prosecco tone. Carries additional information below the first two levels; changes affect bound labels and graphics.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/content/static-dark-primary",
      "description": "Theme-invariant opaque dark text and icons, black by default. Often used over images or other content that stays unchanged when the interface theme switches.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/content/static-dark-secondary",
      "description": "Theme-invariant translucent dark text and icons. Carries secondary information over images or other content that stays unchanged when the interface theme switches.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/content/static-light-primary",
      "description": "Theme-invariant opaque light text and icons, white by default. Often used over images or other content that stays unchanged when the interface theme switches.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/content/static-light-secondary",
      "description": "Theme-invariant translucent light text and icons. Carries secondary information over images or other content that stays unchanged when the interface theme switches.",
      "meaningStatus": "owner-defined"
    }
  ]
}
```
