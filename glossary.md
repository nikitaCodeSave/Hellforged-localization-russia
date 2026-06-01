# Hellforged — Мастер-глоссарий EN → RU

Версия: v1 (черновой эталон). Источник: ru-locale-kit (`abilities`, `stats_enums`, `narrative`, `gear_names`, `ui_meta`, `systems`, `progression`). Уровень уверенности терминов: `confirmed-data` (из извлечённых строк) для EN; RU — рекомендация локализатора (`tentative`), фиксируется как канон после первого ревью.

**Принцип:** один EN-термин = один RU-термин. Колонка «пометка» — род/контекст/предупреждение.

---

## 1. Имена собственные — герои

| EN | RU | Пометка |
|---|---|---|
| Thoren | Торен | паладин, м.р., суровый |
| Mortenzia | Мортензия | тёмная эльфийка, маг, ж.р., высокомерная |
| Paladin (класс) | Паладин | |
| Mage (класс) | Маг | |
| Dark Elf | тёмная эльфийка / тёмный эльф | раса Мортензии |

## 2. Имена собственные — NPC

| EN | RU | Пометка |
|---|---|---|
| The Shade | Тень | мистик, торжественно-зловещий; ж.р. «Тень» |
| Garrick | Гаррик | летописец, сухой сарказм |
| Keldor | Келдор | кузнец, резкий |

## 3. Имена собственные — боссы и существа

| EN | RU | Пометка |
|---|---|---|
| Crypt Prince | Принц склепа | босс |
| Necromancer | Некромант | босс |
| The Executor | Палач | босс (не «Экзекьютор») |
| Dread Presence | Грозное присутствие | модификатор сложности босса |
| Standard Presence | Обычное присутствие | |
| Empowered Presence | Усиленное присутствие | |
| Blood Worms | Кровавые черви | испытание/враги |
| Blood Worm Queen | Королева кровавых червей | |
| Blood Pylon | Кровавый пилон | |
| Blood Tumour / Tumor | Кровавая опухоль | (брит./амер. написание — единый RU) |
| Elite | Элита / элитный | «kill Elites» → «убийство элиты» |
| Boss | Босс | ранг существа |
| Creature Tier | Ранг существа | |

## 4. Названия систем и сущностей мира

| EN | RU | Пометка |
|---|---|---|
| Expedition | Экспедиция | |
| Run | Забег | |
| Stage | Этап | `Stage {n}` → «Этап {n}» |
| Camp | Лагерь | хаб между забегами |
| The Obelisk | Обелиск | механика выхода; с заглавной |
| The Collapse | Коллапс | финальная фаза распада карты |
| Overtime Fog | Туман распада | овертайм-механика |
| Rift | Разлом | запечатывается ради Хаоса/Очков |
| Eternal Tree | Вечное Древо | мета-дерево прокачки; оба слова с заглавной |
| Progression Journey | Путь развития | дерево разблокировок систем |
| Arsenal | Арсенал | пул способностей/реликвий для забега |
| Blacksmith | Кузнец | здание |
| Stash | Хранилище | |
| Salvaging | Разбор | |
| Achievements | Достижения | |
| Archive | Архив | здание (claim achievements) |
| Shrine of Power | Святилище силы | даёт способность |
| Altar of Blessing | Алтарь благословения | |
| Effigy / Effigies | Идол / Идолы | повышают сложность и награды |
| Sigil | Сигил | даёт легендарный выбор |
| Runestone | Рунный камень | захватывается ради XP-радиуса |
| Treasure Chest | Сундук с сокровищами | источник реликвий |
| Locked Chest | Запертый сундук | стоит золота |
| Summoning Ritual | Ритуал призыва | окно призыва босса |
| Build | Сборка | `Builds/Presets` → «Сборки/Пресеты» |
| Preset | Пресет | |

## 5. Редкости (RARITY_*) и качество

| EN | RU | Пометка |
|---|---|---|
| Common | Обычный | редкость |
| Rare | Редкий | |
| Epic | Эпический | |
| Legendary | Легендарный | |
| Mythic | Мифический | вознесение легендарки |
| Unique | Уникальный | |
| Major Affix | Крупный аффикс | |
| Minor Affix | Малый аффикс | |
| Infused | Влитый | постфикс « (Влитый)» |
| Possible Roll | Возможное значение | |

## 6. Крафт / Кузнец (BLACKSMITH_*, ASCEND_*)

| EN | RU | Пометка |
|---|---|---|
| Empower | Усилить | Common/Rare → Legendary |
| Upgrade to Legendary | Улучшить до легендарного | |
| Ascend | Вознести | Legendary → Mythic |
| Ascend to Mythic Rarity | Вознести до мифической редкости | |
| Infuse | Влить | поднимает все свойства предмета |
| Infuse Properties | Влить свойства | |
| Salvage | Разобрать | |
| Bulk Salvage | Разобрать всё / массовый разбор | |

## 7. Ресурсы и валюта (COLLECTIBLE_*)

| EN | RU | Пометка |
|---|---|---|
| Gold | Золото | |
| Chaos | Хаос | ресурс/валюта призыва |
| Chaos Shard | Осколок хаоса | |
| Chaos Level | Уровень хаоса | |
| Dreadstone | Жуткий камень | дроп с захваченных Разломов |
| Eternal Essence | Вечная эссенция | покупка очков Вечного Древа |
| Prism Shard | Осколок призмы | |
| Scrap | Лом | от разбора снаряжения |
| Graystone | Серокамень | |
| Stormsilver | Штормовое серебро | |
| Magnet | Магнит | подбирающий бонус |
| Score | Очки | `+{n} Score` → «+{n} очков» |

## 8. Характеристики (STAT_*) — ядро, единообразно везде

| EN | RU | Пометка |
|---|---|---|
| Attack Damage | Урон атаки | базовый стат (`Base Damage`) |
| All Damage | Весь урон | `+{0} All Damage` → «+{0} ко всему урону» |
| Ability Damage Bonus | Бонус урона способностей | |
| Cast Speed (Bonus) | Скорость каста (бонус) | |
| Attack Speed | Скорость атаки | |
| Attack Range | Дальность атаки | |
| Critical Chance | Шанс крита | (в описаниях допустимо «критический урон» полностью) |
| Critical Damage | Критический урон | |
| Armor | Броня | |
| Armor Percentage Cap | Предел брони (%) | макс. снижение урона |
| Magic Resistance | Сопротивление магии | |
| Max Life | Макс. здоровье | |
| Life Regeneration | Регенерация здоровья | |
| Energy Shield | Энергощит | |
| Absorb | Поглощение | |
| Thorns | Шипы | отражение урона |
| Lifesteal | Вампиризм | (`Lifesteal Chance` → «Шанс вампиризма») |
| Evade / Evasion Chance | Шанс уклонения | |
| Move Speed | Скорость передвижения | |
| Collect Range | Радиус сбора | XP/подбор |
| Area Bonus | Бонус площади | |
| Projectile Count | Кол-во снарядов | |
| Bounce Count | Кол-во отскоков | |
| Duration | Длительность | |
| Radius | Радиус | |
| Range | Дальность | |
| Cooldown | Перезарядка | НЕ «откат» |
| Trigger Chance | Шанс срабатывания | |
| Apply Chance | Шанс наложения | статус-эффекта |
| Spread Chance | Шанс распространения | |
| Gold Gain / Gold Find | Прирост золота / Поиск золота | |
| Experience gain | Прирост опыта | |
| Item Level | Уровень предмета | `Total Item Lvl` → «Сумм. ур. предметов» |

### Базовый урон по школам (Base X Damage)
| EN | RU |
|---|---|
| Base Physical Damage | Базовый физический урон |
| Base Fire Damage | Базовый огненный урон |
| Base Cold Damage | Базовый холодный урон |
| Base Lightning Damage | Базовый урон молнией |
| Base Necrotic Damage | Базовый некротический урон |
| Base Mystic Damage | Базовый мистический урон |
| Base Bleed Damage | Базовый урон кровотечения |
| Base Burn Damage | Базовый урон горения |
| Base Overcharge Damage | Базовый урон Перегрузки |

## 9. Школы урона (ENUM_DAMAGE_CATEGORY_*)

| EN | RU | Пометка |
|---|---|---|
| Physical | Физический | урон |
| Fire | Огонь / огненный | |
| Cold | Холод / холодный | |
| Lightning | Молния | «Lightning damage» → «урон молнией» |
| Necrotic | Некротический | |
| Mystic | Мистический | |
| Shadow | Теневой | |
| Poison | Яд / ядовитый | |
| Burn | Горение | как урон и как статус |
| Bleed | Кровотечение | как урон и как статус |

## 10. Статусы (STATUS_EFFECT_*)

| EN | RU | Пометка |
|---|---|---|
| Bleed | Кровотечение | |
| Blight | Порча | стаки +урон получаемый |
| Burn | Горение | |
| Chill | Озноб | замедление; на макс. → Заморозка |
| Frozen | Заморозка | нельзя двигаться |
| Conductive | Проводимость | дроп зарядов крит-урона |
| Death Curse | Смертельное проклятие | взрыв при смерти |
| Stun | Оглушение | |
| Slow Movement | Замедление | |
| Stack | Заряд | «Max {n} stacks» → «Макс. {n} зарядов» |

## 11. Способности и боевые механики (ABILITY_*)

### Названия способностей (NAME)
| EN | RU | Пометка |
|---|---|---|
| Main Attack | Основная атака | базовый удар; не масштабируется Ability Damage |
| Arcane Missile | Чародейский снаряд | |
| Chasing Lightning | Преследующая молния | |
| Chain Lightning | Цепная молния | морф |
| Deathcoil | Смертельная спираль | |
| Fireball | Огненный шар | |
| Flame Wall | Огненная стена | |
| Flame Ring | Огненное кольцо | морф |
| Frost Orb | Ледяная сфера | |
| Cryo Nova | Криовзрыв | морф |
| Ice Shards | Ледяные осколки | |
| Lightning Orbs | Сферы молний | |
| Meteor | Метеор | |
| Scorched Earth | Выжженная земля | морф |
| Necrotic Surge | Некротический всплеск | |
| Piercing Chains | Пронзающие цепи | |
| Greathammer | Молот-громада | паладин |
| Divine Barrage | Божественный шквал | |
| Hammers of Wrath | Молоты гнева | |
| Judgment Detonation | Подрыв возмездия | морф |
| Lightfall | Падение света | морф |
| Spike Burst | Взрыв шипов | морф |
| Explosive Spikes | Взрывные шипы | морф |
| Burning Discharge | Огненный разряд | морф |
| Conductor's Mark | Метка проводника | морф |
| Concussive Chains | Контузящие цепи | морф |
| Rending Chains | Раздирающие цепи | морф |
| Death Curse | Смертельное проклятие | морф |
| Deathcoil Pool | Лужа смертельной спирали | морф |
| Necrotic Surge Pool | Лужа некротического всплеска | морф |
| Moving Wall | Движущаяся стена | морф |
| Fireball Replication | Расщепление огненного шара | морф |

### Боевые понятия
| EN | RU | Пометка |
|---|---|---|
| Overcharge | Перегрузка | ульта-механика; всегда термин с заглавной |
| Morph | Морф | эволюция способности |
| Trait | Черта | пассивный апгрейд способности |
| Powerup | Усиление | подбираемый бонус в забеге |
| Relic | Реликвия | |
| Dash | Рывок | `Dash Recharge` → «восстановление рывка» |
| Pierce | Пробитие | `pierce count` → «число пробитий» |
| Critical hit / Crit | Критический удар / крит | |
| Status Effect | Статус-эффект | |
| Crowd Control | Контроль | (CC) |
| Haste | Спешка | тег усиления |
| Sustain | Устойчивость | тег (самоподдержка) |
| Economy | Экономика | тег |

## 12. Прогрессия и Вечное Древо (ETERNAL_TREE_*, PROGRESSION_*)

| EN | RU | Пометка |
|---|---|---|
| Node | Узел | «Major/Minor node» → «крупный/малый узел» |
| Major | Крупный | тип узла |
| Minor | Малый | тип узла |
| Specialization | Специализация | тип узла |
| Buy Point | Купить очко | |
| Points Available | Доступно очков | |
| Reset | Сбросить | |
| Ambush (stacks) | Засада (заряды) | механика Ассасина |
| Focus | Сосредоточение | узел/механика |
| Overlife | Сверхздоровье | механика Джаггернаута |
| Shockwave | Ударная волна | |
| Shatter Nova | Раскалывающий взрыв | |
| Vacuum | Вакуум | механика Магнетизма |
| Polarity | Полярность | |
| Coinburst | Монетный залп | механика Гоблина |
| Gold Cap | Предел золота | |

### Архетипы-узлы (имена собственные узлов)
| EN | RU |
|---|---|
| Assassin | Ассасин |
| Goblin | Гоблин |
| Juggernaut | Джаггернаут |
| Magnetism | Магнетизм |
| Challenger's Momentum | Натиск претендента |
| Legend's Dawn | Рассвет легенды |
| Monolith's Promise | Обещание монолита |
| Power of Choice | Сила выбора |

## 13. Лут и забег (онбординг/HUD)

| EN | RU | Пометка |
|---|---|---|
| Loot | Добыча | |
| Loot Safety | Сохранность добычи | первые 3 предмета защищены |
| Secured / Unsecured loot | Защищённая / незащищённая добыча | |
| Exit Portal | Портал выхода | ранний выход с лутом |
| Extract | Извлечь / эвакуироваться | вынести добычу |
| Challenge | Испытание | |
| Offering (Greater/Lesser/Major) | Подношение (Великое/Малое/Большое) | выбор при призыве босса |
| Score Reward | Награда очками | |
| Shade Essence | Эссенция Тени | для морфов |

## 14. UI / меню / настройки (OPTIONS_*, CONTROLS_*, PAUSE_*)

| EN | RU | Пометка |
|---|---|---|
| Options | Настройки | |
| Game / Display / Audio | Игра / Экран / Звук | вкладки |
| Controls | Управление | |
| Aiming (Automatic/Manual) | Прицеливание (Авто/Вручную) | |
| Auto-Attack | Автоатака | |
| Input Hand Mode | Режим руки | Left/Right-handed → Левша/Правша |
| Resolution | Разрешение | |
| Fullscreen | Полный экран | |
| Graphic Quality (High/Low) | Качество графики (Высокое/Низкое) | |
| Special Effect Quality | Качество спецэффектов | Performance/Quality/Ultra → Производительность/Качество/Ультрапроизводительность |
| Anti-Aliasing | Сглаживание | |
| Shadows | Тени | |
| VSync | Верт. синхронизация | |
| Frame Rate Limit | Ограничение кадров | |
| Camera Shake | Тряска камеры | |
| Combat Log | Боевой лог | |
| Damage Meter | Счётчик урона | |
| Show Damage Numbers | Показывать числа урона | |
| Global Volume | Общая громкость | |
| Music / SFX | Музыка / Звук. эффекты | |
| Confine Cursor | Удерживать курсор | |
| Save Slot | Слот сохранения | |
| Create new save | Создать сохранение | |

## 15. Достижения (ENUM_ACHIEVEMENT_CATEGORY_*)

| EN | RU |
|---|---|
| General | Общие |
| Abilities | Способности |
| Morphs | Морфы |
| Relics | Реликвии |
| Lifetime | За всё время |
| Runs | Забеги |
| Feats of Strength | Подвиги |
| Secrets | Секреты |

## 16. Прилагательные/материалы для имён снаряжения (gear NamePools)

Порядок в RU — естественный «прилагательное + существительное», род/число по слоту. Не калькировать, держать тёмное фэнтези.

### Слоты
| EN | RU (м/ж/мн по предмету) |
|---|---|
| Chest (Heavy/Medium/Light) | Нагрудник / доспех / роба |
| Feet | Сапоги / поножи / сабатоны |
| Hands | Перчатки / латные рукавицы |
| Gauntlets | Латные рукавицы |
| Greaves / Sabatons | Поножи / сабатоны |
| Cuirass / Breastplate | Кираса / нагрудник |
| Robe / Vestment / Raiment | Роба / облачение / одеяние |

### Типовые прилагательные (common-tier — потрёпанность)
| EN | RU |
|---|---|
| Worn | Поношенный |
| Weathered | Видавший виды |
| Tarnished | Потускневший |
| Battle-Scarred | Иссечённый в боях |
| Rugged | Грубый |
| Frayed / Threadbare | Истрёпанный / ветхий |
| Scuffed | Потёртый |
| Dust-Laden / Dust-Worn | Запылённый |
| Rustflecked / Rusty | Тронутый ржавчиной |
| Faded | Выцветший |
| Sturdy | Крепкий |
| Plain / Simple | Простой |
| Reinforced / Fortified | Усиленный |
| Hardened / Tempered | Закалённый |

### Эпитеты редкого/легендарного (величие, ад, драконы)
| EN | RU |
|---|---|
| Hellforged | Адокованный |
| Hellwoven | Сотканный в аду |
| Hellclad | Облачённый адом |
| Dragonforged / Dragonscale / Dragonsoul | Драконокованый / Из драконьей чешуи / Драконьей души |
| Emberforged / Ember-Wreathed / Emberblessed | Угольнокованый / Объятый угольями / Благословлённый углём |
| Cinderstorm / Cinderbound / Cinderloom | Пепельный шторм / Скованный пеплом / Тканный пеплом |
| Bloodfire / Bloodsteel | Кроваво-огненный / Кровавая сталь |
| Shadowfire / Shadowbane / Shadowbound | Теневое пламя / Погибель тьмы / Скованный тенью |
| Abyssal | Бездонный / из Бездны |
| Nightfall / Nightveil / Nightguard | Сумеречный / Завеса ночи / Страж ночи |
| Doomsteel / Doomchant / Doomplate | Роковая сталь / Песнь рока / Латы рока |
| Eternal / Immortal | Вечный / Бессмертный |
| Worldbreaker / Worldforged | Сокрушитель миров / Кованый миром |
| Warlord's / Imperator's / Kingsgild | Военачальника / Императора / Королевской позолоты |
| Sanctified / Seraphic / Hierophant | Освящённый / Серафический / Иерофанта |
| Titanshield / Colossus / Apex | Щит титана / Колосс / Вершинный |
| Stormbreaker / Stormthread / Stormwoven | Сокрушитель бурь / Нить бури / Тканный бурей |
| Runebound / Runetouched / Rune-Touched | Скованный рунами / Тронутый рунами |
| Spiritwoven / Hexbound / Hexmarked | Тканный духом / Скованный порчей / Меченый порчей |
| Oathbound | Связанный клятвой |
| Ancestor's | Предка |
| Vanguard / Sentinel / Bastion | Авангарда / Часового / Бастиона |
| Bulwark / Rampart / Aegis | Оплот / Вал / Эгида |

> Имена снаряжения переводятся по смыслу как единая фраза, а не пословно. Пример: «Warlord's Aegis Vest» → «Эгида военачальника»; «Dragonforged Bulwark» → «Драконокованый оплот»; «Worldbreaker Cuirass» → «Кираса сокрушителя миров».

---

## 17. Слова-табу / антипаттерны

| Не писать | Писать |
|---|---|
| Откат, кулдаун | Перезарядка |
| Дамаг, ДМГ | Урон |
| Хелс, хп | Здоровье |
| Лут (как калька в UI) | Добыча |
| Овертайм | Туман распада / Коллапс |
| Уникальный легендарный | по точной редкости |
| Экзекьютор, Уорлдбрейкер | переводить по смыслу |
| Заголовок Каждого Слова | заглавная только в начале |
