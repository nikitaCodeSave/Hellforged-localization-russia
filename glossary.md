# Глоссарий EN→RU для русской локализации Hellforged (эталон для всех переводчиков)

Базируется на `_glossary_seed.md` (не противоречит ему) и расширен полным разбором исходников
(`Content.json`, `NamePools.json`, `UI.json`, `Gameplay.json`, `Dialogue.json`).
Версия данных: снимок `data/raw` от 2026-06-01 (числа/состав привязаны к этому снимку, патч может менять).
Уровень уверенности: имена/термины — `confirmed-data` (из ассетов локализации); художественные эквиваленты предметов — `tentative` (наша реконструкция стиля).

---

## 1. Имена собственные (proper nouns)

### Герои (играбельные)
- Hellforged → **Hellforged** (название игры — НЕ переводить)
- Thoren → **Торен** (герой-паладин, м.р.)
- Mortenzia → **Мортензия** (героиня-маг, ж.р.)
- Paladin (как класс/обращение) → **Паладин**
- Mage (как класс) → **Маг**

### NPC (Лагерь)
- The Shade → **Тень** (NPC; в тексте часто `<1>The Shade</1>` — тег сохранять, внутри «Тень»)
- Garrick → **Гаррик** (NPC-летописец)
- Keldor → **Келдор** (NPC-кузнец; «put the broken things by the anvil»)

### Боссы
- Crypt Prince → **Принц склепа**
- Necromancer → **Некромант**
- The Executor → **Палач** (босс; отличать от достижения «Executioner»)
- Executioner (достижение) → **Палач-каратель** (чтобы не путать с боссом The Executor)

### Локации / карты
- Undercrypt → **Подсклеп** (карта)
- Forsaken Reach → **Покинутые пределы** (карта)
- Camp → **Лагерь**

### Сюжетные пропы
- Corpse of Mortenzia → **Тело Мортензии**
- Exit Portal → **Портал выхода**
- Boss Summoning / Summoning Ritual → **Призыв босса** / **Ритуал призыва**

---

## 2. Системные термины (game systems) — переводить единообразно

- Expedition → **Экспедиция**
- Expedition Mode → **Режим экспедиции**
- Run → **Забег** (один заход в экспедицию; «during a run» → «во время забега»)
- Eternal Tree → **Вечное Древо**
- Progression Journey / Progression Tree → **Путь развития**
- Arsenal → **Арсенал**
- Blacksmith → **Кузнец** (заведение/вкладка)
- Stash → **Хранилище**
- Salvaging / Salvage → **Разбор** / **Разобрать** (распыление снаряжения в Scrap)
- Bulk Salvage → **Разобрать всё**
- Relic → **Реликвия**
- Obelisk → **Обелиск** (`The Obelisk` → «Обелиск»)
- Sigil → **Сигил**
- Runestone → **Рунный камень**
- Rift → **Разлом**
- The Collapse → **Коллапс** (фаза овертайма; «Collapse has ended» → «Коллапс завершился»)
- Overtime → **Овертайм** (фаза усиления врагов)
- Shrine of Power → **Святилище силы**
- Shrine (короткое) → **Святилище**
- Altar of Blessing → **Алтарь благословения**
- Effigy → **Идол** (проп/устройство, поднимающее сложность за Chaos)
- Treasure Chest → **Сундук с сокровищами**
- Trial / Mutated Trial → **Испытание** / **Мутировавшее испытание**
- Challenge → **Челлендж**
- Overcharge → **Перегрузка**
- Gear → **Снаряжение**
- Build → **Билд** (сборка персонажа)
- Preset → **Пресет** (набор арсенала)
- Loot → **Добыча** («keep your loot» → «сохранить добычу»)
- Secured Loot → **Защищённая добыча**; Unsecured Loot → **Незащищённая добыча**
- Extract / Extraction / Extracted → **Извлечь** / **Извлечение** / **Извлечённое**
- Morph → **Морф** (модификация способности; `<1>{morphName}</1>` — тег сохранять)
- Global Morph → **Глобальный морф**; Morph Evolution → **Эволюция морфа**; Evolution Morphs → **Эволюционные морфы**
- Trait → **Трейт**; Focus Trait → **Фокус-трейт**
- Ability → **Способность**
- Powerup → **Усиление** (общий термин для способностей/трейтов/морфов в пикере)
- Legendary Power → **Легендарная сила**
- Main Attack → **Основная атака**
- Dash → **Рывок**
- Stat → **Характеристика**
- Affix → **Аффикс**; Major Affix → **Главный аффикс**; Minor Affix → **Малый аффикс**
- Item Level / Item Lvl → **Уровень предмета**
- Item Power → **Сила предмета**
- Item Type → **Тип предмета**
- Hero Level → **Уровень героя**
- Chaos Level → **Уровень хаоса**
- Score → **Очки** (счёт; «+{scoreAmount} Score» → «+{scoreAmount} очков»)
- High Score → **Рекорд**
- Difficulty → **Сложность**; Normal → **Нормальная**; Hard → **Тяжёлая**
- Leaderboard → **Таблица лидеров**
- Achievement → **Достижение**
- Feats of Strength → **Подвиги** (категория достижений)
- Stage → **Этап** (уровень внутри экспедиции; «Stages: {0}» → «Этапы: {0}»; «Stage {n}» → «Этап {n}»)
- Tier → **Ранг** (Tier III → Ранг III; «Map Tiers» → «Ранги карт»; «Tier I» → «Ранг I»)
- Boss → **Босс**
- Specialization → **Специализация**
- Reforging: Infuse → **Наполнить**; Empower → **Усилить**; Ascend → **Вознести**
- Infusion → **Наполнение**; Ascension → **Вознесение**

### Перегрузка/состояния (Gameplay-эффекты, ст. род — «эффект»)
- Bane → **Проклятие** (негативная половина пакта; «Berserker's Pact Bane» → «Проклятие пакта берсерка»)

---

## 3. Редкости и качества (rarity) — единая система

- Common → **Обычный**
- Rare → **Редкий**
- Epic → **Эпический**
- Legendary → **Легендарный**
- Mythic → **Мифический**
- Corrupted → **Осквернённый**
- Unique → **Уникальный**

### Тиры существ (creature tiers)
- Regular → **Обычный** (враг)
- Elite → **Элитный**
- Champion → **Чемпион**
- Boss → **Босс**

---

## 4. Характеристики (stats) — переводить ДОСЛОВНО и единообразно

### Базовые / ядро
- Attack Damage → **Урон атаки** (базовая характеристика; не путать со «Damage»)
- Maximum Life → **Максимальное здоровье**
- Life → **Здоровье**
- Life Regen Amount → **Восстановление здоровья**
- Life Regen Cooldown → **Перезарядка регена**
- Move Speed → **Скорость передвижения**
- Attack Speed → **Скорость атаки**
- Attack Range → **Дальность атаки**

### Урон
- Damage → **Урон**
- All Damage → **Весь урон**
- Ability Damage Bonus → **Бонус урона способностей**
- Overcharge Damage Bonus → **Бонус урона перегрузки**
- Status Effect Damage Bonus → **Бонус урона эффектов**
- Critical Chance → **Шанс крита**
- Critical Damage → **Критический урон**
- Elite Boss Bonus Damage → **Бонус урона по элитам и боссам**
- Physical / Fire / Cold / Lightning / Necrotic / Mystic ... Damage Bonus → **Бонус урона: физический / огненный / холодный / молнией / некротический / мистический ...**
- Base <X> Damage → **Базовый <X> урон** (Base Fire Damage → «Базовый огненный урон»)

### Защита
- Armor → **Броня**
- Armor Percentage Cap → **Предел брони (%)**
- Magic Resistance → **Магическое сопротивление**
- Magic Resistance Cap → **Предел магического сопротивления**
- Elemental Resistance → **Стихийное сопротивление**
- Damage Reduction → **Снижение урона**
- Damage Taken Increase / Decrease → **Увеличение / Снижение получаемого урона**
- Evade Chance → **Шанс уклонения**; Evade Chance Cap → **Предел шанса уклонения**
- Energy Shield → **Энергощит**
- Energy Shield Recharge Amount / Delay → **Восстановление / Задержка восстановления энергощита**
- Thorns → **Шипы**
- Absorb → **Поглощение**; Hit Absorb Amount/Charges → **Поглощение удара (величина / заряды)**
- Invulnerable → **Неуязвимость**
- Overlife / Overlife Percent → **Сверхздоровье** / **Сверхздоровье (%)**
- Lifesteal Chance → **Шанс вампиризма**

### Мобильность / способности
- Dash Charges / Cooldown / Distance / Speed → **Заряды / Перезарядка / Дальность / Скорость рывка**
- Cooldown → **Перезарядка**
- Cast Speed Bonus → **Бонус скорости каста**
- Cast Time → **Время каста**
- Overcharge Cooldown / Regen → **Перезарядка / Восстановление перегрузки**
- Duration → **Длительность**
- Area Bonus → **Бонус площади**
- Radius → **Радиус**; Range → **Дальность**; Arc Angle → **Угол дуги**
- Projectile Count (Bonus) → **Число снарядов (бонус)**
- Projectile Speed / Range (Bonus) → **Скорость / Дальность снаряда (бонус)**
- Pierce Count → **Число пробитий**; Bounce Count → **Число отскоков**
- Knockback Force → **Сила отбрасывания**

### Эффекты / статусы (stat-bonuses)
- Status Effect Duration Bonus → **Бонус длительности эффектов**
- Status Effect Max Stacks / Stacks → **Макс. стаки / Стаки эффекта**
- Status Apply Chance → **Шанс наложения эффекта**
- Trigger Chance → **Шанс срабатывания**
- Bleed / Burn Duration Bonus → **Бонус длительности кровотечения / горения**
- Main Attack Bleed/Burn/Chill/Blight Chance → **Шанс кровотечения/горения/охлаждения/порчи от основной атаки**

### Экономика / утилита
- Gold Gain → **Прирост золота**
- Enemy Gold Drop Bonus → **Бонус выпадения золота с врагов**
- Magic Find → **Поиск магии**
- Experience Gain Bonus → **Бонус опыта**
- Experience Drop Chance → **Шанс выпадения опыта**
- Collect Range → **Радиус сбора**
- Starting Gold → **Стартовое золото**
- Challenge Gold Bonus → **Бонус золота за челленджи**
- Chest Cost Reduction → **Снижение цены сундуков**
- Free Chest Open Chance → **Шанс бесплатного открытия сундука**
- Secure Slots → **Слоты защиты**
- Legendary Power Choices → **Выбор легендарных сил**
- Sigil / Runestone Capture Radius / Speed Bonus → **Бонус радиуса / скорости захвата сигила / рунного камня**
- Gathering Speed / Yield Bonus → **Бонус скорости / добычи при сборе**

### Прочее
- Diminishing Returns → **Убывающая отдача**
- Additive → **Складываемый**; Multiplicative → **Множительный**
- Base / Final / Total → **Базовое / Итоговое / Всего**
- Modifiers → **Модификаторы**

---

## 5. Типы урона (damage categories) и статусы (status effects)

### Типы урона
- Physical → **Физический**
- Fire → **Огненный**; Burn → **Горение**
- Cold → **Холодный**; Chill → **Охлаждение**; Frozen → **Заморозка**
- Lightning → **Молния**; Conductive → **Проводимость**
- Necrotic → **Некротический**
- Shadow → **Теневой**
- Mystic → **Мистический**
- Poison → **Ядовитый**
- Bleed → **Кровотечение**
- Blight → **Порча**

### Статусные эффекты
- Stun → **Оглушение**
- Slow Movement → **Замедление**
- Death Curse → **Проклятие смерти**

### Теги усилений (powerup tags)
- Area → **Площадь**; Crit → **Крит**; Crowd Control → **Контроль**; Damage → **Урон**;
  Dash → **Рывок**; Economy → **Экономика**; Haste → **Спешка**; Move Speed → **Скорость**;
  Overcharge → **Перегрузка**; Projectile → **Снаряд**; Status Effects → **Эффекты**; Sustain → **Устойчивость**

---

## 6. Враги и существа

- Skeleton → **Скелет** (Skeleton Slayer → «Истребитель скелетов»)
- Spectre → **Призрак** (Spectre Hunter → «Охотник на призраков»)
- Goblin → **Гоблин** (Greed/Hoarding/Overflowing — состояния гоблина: **Жадность / Накопление / Переполнение**)
- Worm / Blood Worms → **Червь / Кровавые черви**
- Tumour (Tumor) → **Опухоль** (челлендж «Tumour Purge» → «Зачистка опухолей»)
- Pylon → **Пилон** (челлендж «Pylons of Blood» → «Пилоны крови»)
- Demon → **Демон**
- Horde → **Орда** (Horde Reaper → «Жнец орды»)
- Elite → **Элита/Элитный** (Elite Hunter → «Охотник на элиту»)

---

## 7. Валюты и ресурсы (currencies / collectibles)

- Gold → **Золото**
- Chaos / Chaos Shard → **Хаос** / **Осколок Хаоса**
- Scrap → **Лом** (из разбора снаряжения)
- Dreadstone → **Камень ужаса** (из захваченных Разломов)
- Graystone → **Серый камень**
- Stormsilver → **Грозовое серебро**
- Prism Shard → **Призменный осколок**
- Eternal Essence → **Вечная эссенция**
- Shade Essence / Essence → **Эссенция Тени** / **Эссенция**
- Currency Cache → **Хранилище валюты**
- Magnet → **Магнит** (подбирает опыт/дроп)
- Food → **Еда** (хил-подбор)
- Experience / XP → **Опыт** / **XP** (сокращение можно оставлять)

---

## 8. Прилагательные и материалы для имён предметов (NamePools, GEAR_*)

Переводить художественно (прил.+сущ., естественный русский порядок), сохраняя тёмное фэнтези.
Ниже — устойчивые эквиваленты повторяющихся компонентов имён, чтобы серии звучали единообразно.

### Прилагательные «изношенности» (common-тир)
- Worn → **истёртый / поношенный**
- Weathered → **обветренный**
- Tarnished → **потускневший**
- Rusted / Rustflecked → **ржавый / в пятнах ржавчины**
- Frayed → **обтрёпанный**
- Threadbare → **протёртый до нитей**
- Scuffed → **потёртый**
- Battered → **побитый**
- Plain / Simple → **простой**
- Dust-Worn / Dust-Laden / Dust-Caked → **запылённый / покрытый пылью**
- Battle-Scarred / Battle-Stained → **в боевых шрамах / в боевых пятнах**
- Hardened → **закалённый**
- Sturdy / Solid → **прочный / крепкий**
- Roughcast / Rough-Hewn / Rough-Bound / Roughspun → **грубый / грубо сработанный**
- Tempered → **закалённый**
- Pitted → **в выщербинах**

### Эпитеты силы (legendary/rare-тир)
- Hellforged / Hell-Forge / Hellclad / Hellwoven → **адокованный / Адова кузня / в адовой броне / адово-тканый**
- Dragonscale / Dragonsoul / Dragonforged → **из драконьей чешуи / драконьей души / выкованный драконом**
- Doom- (Doomplate, Doomgrips, Doomwrought) → **роковой** (Doomplate → «Роковые латы»)
- Abyssal / Abyssforged → **бездонный / выкованный в бездне**
- Shadowfire / Shadowflame / Shadowbane / Shadowbound → **теневой огонь / теневое пламя / погибель теней / связанный тенью**
- Ember- (Emberforged, Embersilk, Ember-Wreathed) → **угольный / тлеющий** (Emberforged → «выкованный в углях»)
- Cinder- (Cinderstorm, Cinderbound, Cinderloom) → **пепельный**
- Bloodfire / Bloodsteel / Bloodbound → **кроваво-огненный / кровавая сталь / связанный кровью**
- Nightfall / Nightveil / Nightbane / Nightguard → **сумеречный / ночная вуаль / погибель ночи / ночная стража**
- Storm- (Stormbreaker, Stormwoven, Stormcaller) → **грозовой**
- Rune- (Runebound, Rune-Touched, Rune-Etched) → **рунный / тронутый рунами / гравированный рунами**
- Hex- (Hexbound, Hexmarked) → **проклятый / меченный порчей**
- Spiritwoven → **сотканный из духа**
- Eternal / Immortal / Ancestor's → **вечный / бессмертный / предковый**
- Sovereign / Imperator's / Kingsgild / Warlord's → **властелинский / императорский / королевской позолоты / военачальника**
- Sanctified / Sacred / Oathbound / Oathbreaker → **освящённый / священный / связанный клятвой / клятвопреступный**
- Seraphic / Hierophant / Archmage / Arcanist → **серафический / иерофанта / архимага / арканиста**
- Voidwrought / Voidtremor → **пустотный / дрожь Пустоты**

### Существительные-слоты (типы предметов)
- Helm / Helmet / Warhelm / Dreadhelm → **шлем / боевой шлем / шлем ужаса**
- Hood / Cowl / Hat → **капюшон / куколь / шляпа**
- Visor / Visage / Mask / Faceguard → **забрало / личина / маска / щиток**
- Crown / Diadem / Circlet / Coronet / Halo → **корона / диадема / венец / коронет / нимб**
- Cuirass / Breastplate / Chestplate / Chestguard → **кираса / нагрудник / нагрудная пластина / нагрудный щиток**
- Hauberk / Brigandine / Lamellar / Mail Coat → **хауберк / бригантина / ламелляр / кольчуга**
- Robe / Vestment / Raiment / Habit / Garb / Surcoat → **мантия / облачение / одеяние / ряса / наряд / сюрко**
- Jack / Jerkin / Tunic / Vest / Coat / Tabard → **куртка / безрукавка / туника / жилет / плащ-кафтан / табард**
- Gauntlets / Handguards / Vambraces / Bracers → **латные перчатки / наручи кистей / поручи / наручи**
- Gloves / Grips / Mitts / Handwraps → **перчатки / хваты / рукавицы / обмотки**
- Greaves / Sabatons / Legplates / Legguards → **поножи / сабатоны / ножные латы / набедренники**
- Boots / Treads / Striders / Footwraps / Sandals / Moccasins → **сапоги / ботинки / шагатели / обмотки / сандалии / мокасины**
- Maul / Warhammer / Sledge / Mallet / Hammer / Crusher → **молот / боевой молот / кувалда / колотушка / молоток / дробитель**
- Ring / Band / Loop / Circlet / Signet / Seal / Sigil → **кольцо / ободок / петля / колечко / печатка / печать / знак**

---

## 9. UI-ярлыки (кратко, в стиле игровых меню)

### Кнопки (инфинитив/повелит.)
- Accept → **Принять**; Confirm → **Подтвердить**; Continue → **Продолжить**; Close → **Закрыть**;
  Cancel → **Отмена**; Leave → **Выйти**; Quit → **Выход**; Resume → **Продолжить**; Restart → **Заново**;
  Give Up → **Сдаться**; Skip → **Пропустить**; Delete → **Удалить**; Create → **Создать**; Claim → **Забрать**;
  Equip → **Экипировать**; Remove → **Убрать**; Learn → **Изучить**; Track → **Отслеживать**;
  Summon → **Призвать**; Activate → **Активировать**; Evolve Now → **Эволюция сейчас**;
  Buy Point → **Купить очко**; Reset → **Сброс**; Salvage → **Разобрать**; Add All → **Добавить всё**;
  Infuse → **Наполнить**; Empower → **Усилить**; Ascend → **Вознести**

### Заголовки окон
- Inventory → **Инвентарь**; Character → **Персонаж**; Details → **Детали**; Options → **Настройки**;
  Achievements → **Достижения**; Stash → **Хранилище**; Arsenal → **Арсенал**; Blacksmith → **Кузнец**;
  Effigy → **Идол**; Leaderboard → **Таблица лидеров**; Expeditions → **Экспедиции**;
  Map Tiers → **Ранги карт**; Treasure Chest → **Сундук с сокровищами**; Equipment → **Снаряжение**

### Подсказки/промпты
- Interact → **Взаимодействие**; Talk → **Говорить**; Begin the Trial → **Начать испытание**;
  Next Stage → **Следующий этап**; Escape to Camp → **Бежать в Лагерь**;
  Loot Acquired → **Добыча получена**; Loot Safety → **Сохранность добычи**;
  Recommended Stats → **Рекомендуемые характеристики**; Run Powers → **Силы забега**;
  Run Stages → **Этапы забега**; New High Score → **Новый рекорд**; Charged → **Заряжен**;
  Auto-Attack Enabled / Disabled → **Автоатака включена / выключена**;
  Difficulty increase → **Сложность повышена**; Overcharge Ready → **Перегрузка готова**

### Сортировки / категории
- By Acquisition / Rarity / Item Type / Item Level / Item Power → **По получению / редкости / типу / уровню предмета / силе предмета**
- Categories → **Категории**; Tags → **Теги**; Presets → **Пресеты**; Summary → **Сводка**; Tracked → **Отслеживается**

### Настройки (Options)
- Display → **Экран**; Audio → **Звук**; Game → **Игра**; Resolution → **Разрешение**;
  Fullscreen → **Полный экран**; VSync → **Верт. синхр.**; Anti-Aliasing → **Сглаживание**;
  Shadows → **Тени**; Music → **Музыка**; SFX → **Звуки**; Global Volume → **Общая громкость**;
  Damage Meter → **Счётчик урона**; Combat Log → **Боевой журнал**; Language → **Язык**;
  Show Damage Numbers → **Показывать цифры урона**; Camera Shake → **Тряска камеры**

### Единицы (НЕ переводить интернациональные)
- DPS → **DPS**; m → **м**; m/s → **м/с**; s → **с**; % → **%**; xp → **опыт** (или оставить «xp» в формулах)
- d / h / m (дни/часы/минуты в таймере) → **д / ч / м**

---

## Правила сохранения {плейсхолдеров} и <разметки> (обязательны для ВСЕХ строк)

1. **Плейсхолдеры в фигурных скобках — `{0}`, `{name}`, `{rewardAmount}`, `{mapName}`, `{challengeName}`,
   `{damageAmount}`, `{damageType}`, `{currencyName}`, `{morphName}`, `{linkedStatName}` и т.п. — сохранять
   ДОСЛОВНО**: не переводить, не менять имя аргумента, не трогать формат-спецификаторы
   (`{timeLimit:N0}`, `{value}d`). Порядок плейсхолдеров в строке можно переставлять под русскую грамматику.
2. **Любые `<...>`-теги сохранять как есть** и в том же количестве: `<b>…</b>`, `<1>…</1>`, `<2>…</2>`,
   `<t0>…</t0>`, `<style=…>`, `<color=…>`, `<sprite=…>`. Открывающий и закрывающий тег должны обрамлять
   соответствующий по смыслу русский фрагмент (как в оригинале обрамляли английский).
3. **Управляющие клавиши/спрайты — `[W0]`, `[…]` — сохранять дословно** (это привязки кнопок).
4. **Переводы строк `\n` (и `\\n` в JSON-экранировании) — сохранять** на тех же местах.
5. Имена предметов (NamePools, ключи `GEAR_*`) — художественно, прил.+сущ., естественный русский порядок;
   единообразие компонентов брать из раздела 8.
6. UI-строки — кратко; кнопки — инфинитив/повелительное наклонение (раздел 9).
7. Тон диалогов — живой, разговорный; беречь характер: Гаррик — ворчливо-тёплый, Тень — загадочно-мрачный,
   Келдор — суровый кузнец, Мортензия — холодно-надменная, Торен — стойкий паладин.
8. Кавычки — русские «ёлочки» в обычном тексте.
9. Род/число имён собственных: Торен — м.р., Мортензия — ж.р., Тень — ж.р. (согласовывать прилагательные
   и глаголы прошедшего времени соответственно).
10. Числа/значения не переводятся; единицы из раздела 9.
