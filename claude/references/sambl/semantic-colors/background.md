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
    "key": "background",
    "title": "Тональные подложки — background",
    "purpose": "Выраженные и спокойные заливки, которые помогают выделять или группировать содержимое выбранным тоном.",
    "constraints": [
      "High и low различают выраженность заливки, а не высоту или положение поверхности.",
      "Изменение background-роли не меняет автоматически её content-пару или компоненты с прямыми palette bindings.",
      "Static-подложки сохраняют одинаковый цвет и прозрачность в Light/Dark; обратный neutral-high-inverted является отдельным назначением."
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
      "path": "colors/background/absinthe-high",
      "description": "Strong background in the Absinthe tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/absinthe-low",
      "description": "Quiet background in the Absinthe tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/brand-extra-high",
      "description": "Strong background in the additional brand tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/brand-extra-low",
      "description": "Quiet background in the additional brand tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/brand-high",
      "description": "Strong background in the main brand tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/brand-low",
      "description": "Quiet background in the main brand tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/curacao-high",
      "description": "Strong background in the Curacao tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/curacao-low",
      "description": "Quiet background in the Curacao tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/negroni-high",
      "description": "Strong background in the Negroni tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/negroni-low",
      "description": "Quiet background in the Negroni tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/neutral-high",
      "description": "Strong background in the neutral tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/neutral-high-inverted",
      "description": "Strong neutral background with the opposite lightness to the usual high treatment. Changes the fill of the contrasting block; its content color is chosen separately.",
      "meaningStatus": "proposed-interpretation"
    },
    {
      "path": "colors/background/neutral-low",
      "description": "Quiet background in the neutral tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/prosecco-high",
      "description": "Strong background in the Prosecco tone. Makes a colored block more prominent; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/prosecco-low",
      "description": "Quiet background in the Prosecco tone. Gently groups content with less visual weight; changes affect bound surfaces, while their content color needs a separate check.",
      "meaningStatus": "documented-use"
    },
    {
      "path": "colors/background/static-dark-high",
      "description": "Theme-invariant opaque dark background, black by default. Keeps the surface appearance unchanged when the interface theme switches; its content color is chosen separately.",
      "meaningStatus": "owner-defined"
    },
    {
      "path": "colors/background/static-light-high",
      "description": "Theme-invariant opaque light background, white by default. Keeps the surface appearance unchanged when the interface theme switches; its content color is chosen separately.",
      "meaningStatus": "owner-defined"
    }
  ]
}
```
