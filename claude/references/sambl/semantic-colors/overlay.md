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
    "key": "overlay",
    "title": "Прозрачные наложения — overlay",
    "purpose": "Тонировка с сохранением участия нижележащего фона. Её результат зависит от подложки; роль сама не задаёт interaction state.",
    "constraints": [
      "Видимый результат зависит от нижележащей поверхности и прозрачности выбранного цвета.",
      "Тональный overlay не равен floor-overlay, modal scrim или слоту Overlay в Main Layout.",
      "Изменение роли само не создаёт blur и не перенастраивает все hover/pressed: некоторые состояния используют другие связи.",
      "Static light/dark overlays сохраняют одинаковый цвет и прозрачность в Light/Dark, в том числе поверх изображений и другого содержимого, не зависящего от темы."
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
      "path": "colors/overlay/absinthe",
      "description": "Translucent overlay in the Absinthe tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/brand",
      "description": "Translucent overlay in the main brand tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/brand-extra",
      "description": "Translucent overlay in the additional brand tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/curacao",
      "description": "Translucent overlay in the Curacao tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/negroni",
      "description": "Translucent overlay in the Negroni tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/neutral",
      "description": "Translucent overlay in the neutral tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/prosecco",
      "description": "Translucent overlay in the Prosecco tone. Tints a surface together with its underlying background; changes affect the strength and character of the tint without defining an interaction state.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/overlay/static-dark",
      "description": "Theme-invariant translucent dark overlay. Dims images or other underlying content while retaining the same color and opacity when the interface theme switches.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/overlay/static-light",
      "description": "Theme-invariant translucent light overlay. Lightens images or other underlying content while retaining the same color and opacity when the interface theme switches.",
      "meaningStatus": "owner-defined"
    }
  ]
}
```
