# Hellforged — Russian (ru) localization kit

Community-prepared **Russian translation** for **Hellforged** (Unity Localization), packaged so the
team can drop it into the existing project with minimal effort. Every string is keyed by the game's
**real** localization `Key`/`Id` (extracted from the shipped `SharedTableData`), so it imports straight
into the matching String Table Collections.

> ⚠️ The Russian text is a **machine-assisted DRAFT** for your review, not a finished human translation.
> Placeholders (`{0}`, `{rewardAmount}`) and rich-text tags (`<sprite=…>`, `<style=…>`, `<b>`) are
> preserved. See [QA_REPORT.md](QA_REPORT.md) for an automated placeholder/markup sanity check.
> See [DISCLAIMER.md](DISCLAIMER.md) for provenance.

## What's inside

```
csv/                 One CSV per String Table Collection — Unity Localization import format
  Common.csv  System.csv  UI.csv  Gameplay.csv  Dialogue.csv  NamePools.csv  Content.csv
xlsx/
  hellforged-ru.xlsx  Same data, one sheet per collection (+ _index) — for Google Sheets / review
glossary.md          EN→RU term & proper-noun glossary used for consistency (review reference)
QA_REPORT.md         Placeholder / markup preservation check + translated coverage
DISCLAIMER.md        Provenance & licensing note
```

Columns in every CSV / sheet: **`Key`**, **`Id`**, **`English(en)`**, **`Russian(ru)`**.
`Key` and `Id` are the stable identifiers from your `SharedTableData` (the same across all languages),
so the rows line up with your existing collections 1:1. `English(en)` is included only as a review aid.

## The 7 collections (≈1989 strings)

| Collection | Strings | Content |
|---|---|---|
| Common | 4 | Buttons / shared words |
| System | 1 | System message |
| UI | 557 | Interface labels, stat names (has `{0}` placeholders) |
| Gameplay | 85 | In-run prompts / labels |
| Dialogue | 86 | NPC dialogue lines |
| NamePools | 336 | Procedural gear names (`GEAR_*`) |
| Content | 920 | Names, lore, descriptions, tiers |

## How to add Russian to the game (Unity Localization)

You already own the source project, the `com.unity.localization` package, and the 7 String Table
Collections — so the structural work is trivial; this kit supplies the **translated strings**.

1. **Add the Russian Locale.**
   `Window ▸ Asset Management ▸ Localization Tables ▸ Locale Generator` → check **Russian (ru)** → Add.
   (Or create a `Locale` asset with `LocaleIdentifier` code `ru`; set its **Fallback Locale → English**,
   mirroring the other 8 languages.)

2. **Import the translations** into each String Table Collection.
   Open a collection (e.g. **UI**) → the **⋮** menu (top-right of the table editor) → **Import ▸ CSV…** →
   pick `csv/UI.csv`. In the column-mapping dialog, map the **`Russian(ru)`** column to the **ru** locale,
   keyed by **`Key`** (or `Id`). Repeat for all 7 collections.
   - No CSV extension installed? Add **com.unity.localization** sample *“CSV Extension”*, or use
     `xlsx/hellforged-ru.xlsx` via the official **Google Sheets** extension, or paste the `Russian(ru)`
     column directly in the table editor.
   - Untranslated/empty keys are fine — they fall back to English at runtime (same as your CJK languages).

3. **Fonts — Cyrillic already works, no atlas baking needed.**
   The global UI font (`Spectral`, static) has no Cyrillic, but its TMP **fallback chain** starts with the
   **dynamic** `NotoSans…` font whose embedded source TTF contains the full Cyrillic block (U+0400–04FF).
   Cyrillic renders on demand exactly the way your JP/KR/ZH text already does. *Verify in a TMP field once.*
   - Cosmetic only: title font `Cinzel` (static) has no Cyrillic, so Russian titles fall through to Noto
     Sans (style mismatch, not a missing-glyph bug). Add Cyrillic to the title font if you care.

4. **List Russian in the language menu.**
   Add a `LanguageOption` for `ru` to the **`LocalizationDatabase`** asset (the `languages` list that drives
   the settings dropdown): `localeCode: "ru"`, `nativeName: "Русский"`, `releaseState: Released`,
   `sortOrder: 900`. The menu is gated on **both** this entry **and** the `ru` Locale being in
   `AvailableLocales`.

5. **Build Addressables** (your Localization groups). Unity regenerates the `ru` string-table bundle and the
   content catalog automatically — no manual catalog editing.

That's it: launch, pick **Русский** in settings, verify Cyrillic renders.

## Reviewing the draft

- Start with [glossary.md](glossary.md) — fix any term you'd render differently, then it's a find/replace.
- [QA_REPORT.md](QA_REPORT.md) flags rows where a `{placeholder}` or `<tag>` may not have survived — check those first.
- `NamePools` (gear names) and `Dialogue` are the most style-sensitive; `UI`/`Gameplay` are the most
  correctness-sensitive (placeholders).

Questions or a re-export against a newer build are easy to regenerate — the kit is produced by a small,
re-runnable pipeline from the game's own string tables.
