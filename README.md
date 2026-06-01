# Hellforged — Russian (ru) Localization Kit

A drop-in **Russian translation** for **Hellforged**, packaged for Unity Localization so your team can
add the language with minimal effort. Every string is keyed by the game's **own** localization `Key` and
`Id` (read from the shipped `SharedTableData`), so the rows line up 1:1 with your existing String Table
Collections — no remapping, no guesswork.

- **1989 strings**, **100% translated**, across all 7 collections.
- **0 placeholder / markup mismatches** (verified — see [QA_REPORT.md](QA_REPORT.md)).
- Built to a shared [STYLE_GUIDE.md](STYLE_GUIDE.md) + [glossary.md](glossary.md) for consistency.

> **Status:** this is an **AI-produced translation intended for your review**, not a final human
> localization. It was produced in two passes — domain-specialised translators followed by a senior
> game-localization editor per domain — but it should be proofread before shipping. Per-domain editor
> decisions and open questions are documented in [TRANSLATION_NOTES.md](TRANSLATION_NOTES.md).
> Provenance and licensing intent: [DISCLAIMER.md](DISCLAIMER.md).

---

## Contents

```
csv/                    One CSV per String Table Collection — Unity Localization import format
  Common.csv  System.csv  UI.csv  Gameplay.csv  Dialogue.csv  NamePools.csv  Content.csv
xlsx/
  hellforged-ru.xlsx    Same data, one sheet per collection (+ _index) — for Google Sheets / review
STYLE_GUIDE.md          RU style guide: register, industry conventions, plurals, punctuation
glossary.md             EN→RU term & proper-noun glossary used across the whole translation
TRANSLATION_NOTES.md    Per-domain editor decisions & open questions (review aid)
QA_REPORT.md            Placeholder/markup preservation check + coverage
DISCLAIMER.md           Provenance & licensing note
```

Every CSV and sheet has the same four columns:

| Column | Meaning |
|---|---|
| `Key` | The string's human key from `SharedTableData` (e.g. `UI_CONFIRM_BUTTON`) — stable across languages |
| `Id` | The numeric `keyId` (same id used by every locale) |
| `English(en)` | Source text — included only as a review aid |
| `Russian(ru)` | The translation to import |

Files are **UTF-8**, RFC-4180 quoted (multi-line strings and commas handled). Import keyed by `Key` **or**
`Id` — both are authoritative and identical to your project's.

### The 7 collections

| Collection | Strings | What it is |
|---|---|---|
| `Common` | 4 | Shared buttons / words |
| `System` | 1 | System message |
| `UI` | 557 | Interface labels, stat names, tooltips (contains `{0}`-style placeholders) |
| `Gameplay` | 85 | In-run prompts / labels |
| `Dialogue` | 86 | NPC dialogue lines |
| `NamePools` | 336 | Procedurally-named gear (`GEAR_*`) |
| `Content` | 920 | Ability/relic/boss names, lore, descriptions, tiers |

---

## Quick start

1. Add a **Russian (ru)** Locale (Fallback → English).
2. For each of the 7 collections: **Import ▸ CSV** → pick `csv/<Collection>.csv` → map the `Russian(ru)` column.
3. Add a `ru` entry to the `LocalizationDatabase.languages` list so it shows in the settings menu.
4. Build Addressables. Done — fonts already support Cyrillic (see below).

---

## Step-by-step (Unity Localization)

You already own the source project, the `com.unity.localization` package, and the 7 String Table
Collections — so the structural work is trivial. This kit supplies the **translated strings**.

### 1. Add the Russian Locale
`Window ▸ Asset Management ▸ Localization Tables ▸ Locale Generator` → check **Russian (ru)** → **Add Locales**.
Then set the new Locale's **Fallback Locale → English** (mirroring the other 8 languages), so any
untranslated key falls back to English at runtime.

### 2. Import the translations
For each collection, open it in the **Localization Tables** window → **⋮** (top-right) → **Import ▸ CSV…** →
choose the matching `csv/<Collection>.csv`. In the mapping dialog, map the **`Russian(ru)`** column to the
**ru** locale, keyed by **`Key`** (or `Id`).

Alternatives if the CSV importer isn't available:
- Add the **CSV Extension** sample from the `com.unity.localization` package, **or**
- Use `xlsx/hellforged-ru.xlsx` with the official **Google Sheets** extension, **or**
- Paste the `Russian(ru)` column straight into the table editor.

### 3. Fonts — Cyrillic already renders, no atlas baking
The global UI font (`Spectral`, a static atlas) has no Cyrillic glyphs, **but** its TMP fallback chain
begins with a **dynamic** `NotoSans…` font whose embedded source TTF contains the full Cyrillic block
(U+0400–U+04FF). Cyrillic is rasterised on demand at runtime — exactly how your JP/KR/ZH text already
works. No new font asset or atlas baking is required; just confirm a Cyrillic string renders once.

*Cosmetic note:* the title font `Cinzel` (static) lacks Cyrillic, so Russian titles fall through to Noto
Sans. That's a style difference, not a missing-glyph bug — add Cyrillic to the title font only if you want
the exact display style.

### 4. List Russian in the language menu
Add a `LanguageOption` to the **`LocalizationDatabase`** asset's `languages` list (this drives the settings
dropdown):

```
localeCode:    "ru"
nativeName:    "Русский"
releaseState:  Released
sortOrder:     900
```

The language appears only when **both** this entry exists **and** the `ru` Locale is in `AvailableLocales`.

### 5. Build Addressables
Rebuild your Localization Addressables groups. Unity regenerates the `ru` string-table bundle and the
content catalog automatically — no manual catalog editing.

Launch, pick **Русский** in settings, and confirm Cyrillic renders.

---

## Reviewing before you ship

- **Terminology:** [glossary.md](glossary.md) is the single source of truth. Change a term there, then a
  global find/replace keeps every collection consistent.
- **Editor notes:** [TRANSLATION_NOTES.md](TRANSLATION_NOTES.md) lists the non-obvious decisions per domain
  (resolved term collisions, register choices, places that need a human eye).
- **Highest-value proofreading:** `NamePools` (gear flavour) and `Dialogue` (voice) are the most
  style-sensitive; `UI` / `Gameplay` are the most correctness-sensitive (placeholders).
- **Integrity check:** [QA_REPORT.md](QA_REPORT.md) confirms every `{placeholder}`, SmartFormat plural and
  `<tag>` is preserved (currently 0 issues). Re-run it yourself any time with `python verify.py` — it checks
  headers, completeness, placeholder/markup parity, unique ids and CSV↔xlsx consistency. A `pre-push` git
  hook (`.githooks/pre-push`, enabled via `git config core.hooksPath .githooks`) runs it automatically before
  every push.

---

## Verified against the shipped game

This kit was cross-checked against the game's own localization data, not just self-consistency:

- **Keys & ids are exact.** All 1989 `(Key, Id)` pairs were diffed against the live `SharedTableData`
  in the shipped build — **0 mismatches**. Import by `Key` or `Id` lands on the correct existing entries.
- **Coverage.** The kit contains every key that has English source text (1989). A handful of keys with
  no English string are intentionally omitted (nothing to translate; they fall back to English).
- **Smart strings need no special handling.** The game does **not** store an `IsSmart` flag per entry —
  every English entry ships with *empty* metadata, yet 74 of them use SmartFormat syntax (named
  placeholders, `{amount:plural:…}`). SmartFormat is applied globally by the String Database. So the
  imported Russian entries behave exactly like English ones with no extra flag, tag or column.
- **Russian plurals are locale-driven.** SmartFormat picks the plural form from the locale's culture.
  With locale code **`ru`**, `{n:plural:осколок|осколка|осколков}` resolves to the correct Slavic
  1 / few / many form automatically — the translation already provides all three forms where needed.
- **Locale conventions match the existing 9 languages.** Name pattern `"<English> (<code>)"`,
  fallback → English, `releaseState: Released`. Recommended: Locale name **"Russian (ru)"**, code **`ru`**,
  `LocalizationDatabase` `nativeName: "Русский"`.
- **The only entry metadata in the game** is an optional `Comment` (`MT_REVIEW`) used to mark
  machine-translated lines for review — not required, and not included here.

The reproducible checks live in `verify.py` (run on every push via the `pre-push` hook).

## How this was produced

The English strings and their keys were read from the shipped Hellforged build's Unity Localization
tables, then translated in a structured pipeline: a lead linguist established the style guide + master
glossary; the strings were grouped into 8 thematic domains (gear names, abilities, stats, achievements,
progression, systems, narrative, UI); each domain was translated by context-aware translators and then
revised by a senior game-localization editor. An automated check verifies key/id integrity and
placeholder/markup preservation. See [DISCLAIMER.md](DISCLAIMER.md) for the full provenance note.

If you change anything in the source strings or ship a new build, the kit can be regenerated against the
updated tables.
