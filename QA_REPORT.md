# QA report — сохранность плейсхолдеров и разметки

Всего строк: **1989**, переведено: **1989**, пропущено: **0**.

## ⚠️ Несовпадение токенов {...}/<...> (3)
Плейсхолдер или тег в русском не совпадает с английским — проверить вручную:

- **UI/TREASURE_CHEST_COLLECT_ESSENCE_INFO**
  - en: `Collect Essence to summon The Shade`
  - ru: `Соберите эссенцию, чтобы призвать <1>Тень</1>`
- **UI/TREASURE_CHEST_FIND_SHADE_INFO**
  - en: `Find The Shade to choose ability Morph`
  - ru: `Найдите <1>Тень</1>, чтобы выбрать морф способности`
- **Content/RESOURCE_CHAOS_SHARD_AMOUNT_FORMAT**
  - en: `{amount:plural:{} Chaos Shard|{} Chaos Shards}`
  - ru: `{amount:plural:{} Осколок Хаоса|{} Осколка Хаоса|{} Осколков Хаоса}`
